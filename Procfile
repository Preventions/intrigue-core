resolver: bundle exec ruby ./util/resolver.rb
#chrome: /Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --headless --disable-gpu --disable-dev-shm-usage --ignore-certificate-errors --disable-popup-blocking --disable-translate --remote-debugging-port=9222
#tika: java -jar ./tmp/tika-server-1.22.jar
worker: bundle exec sidekiq -C ./config/sidekiq.yml -r ./core.rb
web: bundle exec puma -C ./config/puma.rb -b tcp://127.0.0.1:7777
