
require 'yaml'
require 'deep_merge'

# Load default configuration
config_file = File.expand_path "sculpin.yml.dist"
config = YAML::load(File.open(config_file))

# Load local configuration (if it exists)
localconfig_file = File.expand_path "sculpin.yml"
config.deep_merge! YAML::load(File.open(localconfig_file)) if File.exists?(localconfig_file)

preview_root          = config['preview_destination']
preview_url           = config['preview_url']

deploy_root           = config['destination']

def ok_failed(condition)
  if (condition)
    puts "OK"
  else
    puts "FAILED"
  end
end

desc "Deploy website"
task :deploy do

  deploy_ssh_target     = config['deploy']['ssh']['target']
  begin
    deploy_ssh_port       = config['deploy']['ssh']['port']
  rescue
    deploy_ssh_port       = 22
  end
  deploy_remote_path    = config['deploy']['remote_path']

  ok_failed system "sculpin generate --destination=#{deploy_root}"
  ok_failed system "rsync -avze 'ssh -p #{deploy_ssh_port}' #{deploy_root}/ #{deploy_ssh_target}:#{deploy_remote_path}"

end

desc "Preview website locally"
task :preview do
    system "sculpin generate --watch --url=#{preview_url} --destination=#{preview_root}"
end
