
heroku create -a ktrz-nx-photos-api-2


heroku buildpacks:add -a ktrz-nx-photos-api-2 heroku/nodejs


heroku buildpacks:add -a ktrz-nx-photos-api-2 heroku-community/multi-procfile


heroku config:set -a ktrz-nx-photos-api-2 PROCFILE=apps/photo/api/Procfile


heroku config:set -a ktrz-nx-photos-api-2 PROJECT_NAME=photo-api