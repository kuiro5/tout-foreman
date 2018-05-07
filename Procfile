/*core: sh -c "cd ~/code/tout && env RBENV_VERSION=1.8.7-p375 rbenv exec bundle exec unicorn_rails -p 3000 -c ../../core_unicorn.cfg"*/
core_worker: sh -c "cd ~/code/tout && env RBENV_VERSION=1.8.7-p375 RAILS_ENV=development QUEUE=* COUNT=5 rbenv exec bundle exec rake resque:workers"
core_scheduler: sh -c "cd ~/code/tout && env RBENV_VERSION=1.8.7-p375 RAILS_ENV=development QUEUE=* rbenv exec bundle exec rake resque:scheduler"
next: sh -c "cd ~/code/tout-next && . $(brew --prefix nvm)/nvm.sh && nvm use v0.10.40 && brunch watch --server"
elasticsearch: sh -c "cd ~/code/elasticsearch-0.90.12/bin && ../elasticsearch -f"
elasticsearch5: sh -c "cd ~/code/elasticsearch-5.3.2/bin && ../elasticsearch"
kibana: sh -c 'cd ~/code/kibana-5.3.2-darwin-x86_64/bin && ../kibana'
