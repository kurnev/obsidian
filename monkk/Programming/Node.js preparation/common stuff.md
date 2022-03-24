Delegate all CPU intensive stuff to reverse proxy like nginx for ssl or gzip

npm shrinwrap or yarn
nodejs sits on juts one core

auth token JWT + refresh_token is a way to go

regex can be heavy on CPU, so use good libraires 

setImmediate fires on event loop cycle, whilst process.nextTick() fires after current operation is over, disregarding event loop