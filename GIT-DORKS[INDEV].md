# git dorks 

generic keywords 

password
dbpassword
dbuser
access_key
secret_access_key
bucket_password
redis_password
root_password

search process 

search within target repo or general target keyword 
e.g. 

search by DB name - modified 

or 

site:github - best op > can automate this 

 Dork                                           | Description
------------------------------------------------|--------------------------------------------------------------------------
filename:.npmrc _auth                           | npm registry authentication data
filename:.dockercfg auth                        | docker registry authentication data
extension:pem private                           | private keys
extension:ppk private                           | puttygen private keys
filename:id_rsa or filename:id_dsa              | private ssh keys
extension:sql mysql dump                        | mysql dump
extension:sql mysql dump password               | mysql dump look for password; you can try varieties
filename:credentials aws_access_key_id          | might return false negatives with dummy values
filename:.s3cfg                                 | might return false negatives with dummy values
filename:wp-config.php                          | wordpress config files
filename:.htpasswd                              | htpasswd files
filename:.env DB_USERNAME NOT homestead         | laravel .env (CI, various ruby based frameworks too)
filename:.env MAIL_HOST=smtp.gmail.com          | gmail smtp configuration (try different smtp services too)
filename:.git-credentials                       | git credentials store, add NOT username for more valid results
PT_TOKEN language:bash                          | pivotaltracker tokens
filename:.bashrc password                       | search for passwords, etc. in .bashrc (try with .bash_profile too)
filename:.bashrc mailchimp                      | variation of above (try more variations)
filename:.bash_profile aws                      | aws access and secret keys
rds.amazonaws.com password                      | Amazon RDS possible credentials
extension:json api.forecast.io                  | try variations, find api keys/secrets
extension:json mongolab.com                     | mongolab credentials in json configs
extension:yaml mongolab.com                     | mongolab credentials in yaml configs (try with yml)
jsforce extension:js conn.login                 | possible salesforce credentials in nodejs projects
SF_USERNAME salesforce                          | possible salesforce credentials
filename:.tugboat NOT _tugboat                  | Digital Ocean tugboat config
HEROKU_API_KEY language:shell                   | Heroku api keys
HEROKU_API_KEY language:json                    | Heroku api keys in json files
filename:.netrc password                        | netrc that possibly holds sensitive credentials
filename:_netrc password                        | netrc that possibly holds sensitive credentials
filename:hub oauth_token                        | hub config that stores github tokens
filename:robomongo.json                         | mongodb credentials file used by robomongo
filename:filezilla.xml Pass                     | filezilla config file with possible user/pass to ftp
filename:recentservers.xml Pass                 | filezilla config file with possible user/pass to ftp
filename:config.json auths                      | docker registry authentication data
filename:idea14.key                             | IntelliJ Idea 14 key, try variations for other versions
filename:config irc_pass                        | possible IRC config
filename:connections.xml                        | possible db connections configuration, try variations to be specific
filename:express.conf path:.openshift           | openshift config, only email and server thou
filename:.pgpass                                | PostgreSQL file which can contain passwords
filename:proftpdpasswd                          | Usernames and passwords of proftpd created by cpanel
filename:ventrilo_srv.ini                       | Ventrilo configuration
[WFClient] Password= extension:ica              | WinFrame-Client infos needed by users to connect toCitrix Application Servers
filename:server.cfg rcon password               | Counter Strike RCON Passwords
JEKYLL_GITHUB_TOKEN                             | Github tokens used for jekyll
filename:.bash_history                          | Bash history file
filename:.cshrc                                 | RC file for csh shell
filename:.history                               | history file (often used by many tools)
filename:.sh_history                            | korn shell history
filename:sshd_config                            | OpenSSH server config
filename:dhcpd.conf                             | DHCP service config
filename:prod.exs NOT prod.secret.exs           | Phoenix prod configuration file
filename:prod.secret.exs                        | Phoenix prod secret
filename:configuration.php JConfig password     | Joomla configuration file
filename:config.php dbpasswd                    | PHP application database password (e.g., phpBB forum software)
path:sites databases password                   | Drupal website database credentials
shodan_api_key language:python                  | Shodan API keys (try other languages too)
filename:shadow path:etc                        | Contains encrypted passwords and account information of new unix systems
filename:passwd path:etc                        | Contains user account information including encrypted passwords of traditional unix systems
extension:avastlic "support.avast.com"          | Contains license keys for Avast! Antivirus
filename:dbeaver-data-sources.xml               | DBeaver config containing MySQL Credentials
filename:.esmtprc password                      | esmtp configuration
extension:json googleusercontent client_secret  | OAuth credentials for accessing Google APIs
HOMEBREW_GITHUB_API_TOKEN language:shell        | Github token usually set by homebrew users
xoxp OR xoxb                                    | Slack bot and private tokens
.mlab.com password                              | MLAB Hosted MongoDB Credentials
filename:logins.json                            | Firefox saved password collection (key3.db usually in same repo)
filename:CCCam.cfg                              | CCCam Server config file
msg nickserv identify filename:config           | Possible IRC login passwords
filename:settings.py SECRET_KEY                 | Django secret keys (usually allows for session hijacking, RCE, etc)
filename:secrets.yml password                   | Usernames/passwords, Rails applications
filename:master.key path:config                 | Rails master key (used for decrypting `credentials.yml.enc` for Rails 5.2+)
filename:deployment-config.json                 | Created by sftp-deployment for Atom, contains server details and credentials
filename:.ftpconfig                             | Created by remote-ssh for Atom, contains SFTP/SSH server details and credentials
filename:.remote-sync.json                      | Created by remote-sync for Atom, contains FTP and/or SCP/SFTP/SSH server details and credentials
filename:sftp.json path:.vscode                 | Created by vscode-sftp for VSCode, contains SFTP/SSH server details and credentails
filename:sftp-config.json                       | Created by SFTP for Sublime Text, contains FTP/FTPS or SFTP/SSH server details and credentials
filename:WebServers.xml                         | Created by Jetbrains IDEs, contains webserver credentials with encoded passwords ([not encrypted!](https://intellij-support.jetbrains.com/hc/en-us/community/posts/207074025/comments/207034775))
