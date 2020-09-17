# Set up steps 

# If you don't already have it, install laravel installer
1. composer global require laravel/installer
2. echo 'export PATH="$PATH:$HOME/.composer/vendor/bin"' >> ~/.bashrc
3. source ~/.bashrc

# Create new laravel project
4. laravel new jetshow --jet
5. Create mysql database with name of project 
6. edit app name in .env
7. php artisan migrate
8. npm install && npm run dev

# Set up git repo

7. Create repo on gibhug
8. Run commands `git init && git remote add origin https://github.com/jimtaylor123/jetshow.git && git add . && git commit -m 'initial commit' && git push -u origin master`

# Set up email and file storage, sanity test
9. Configure email in .env with mailtrap values
10. Configure file system in .env e.g.

```env
FILESYSTEM_DRIVER=s3

AWS_ACCESS_KEY_ID=AKIASXWEKEPYUITYWSHKP
AWS_SECRET_ACCESS_KEY=BMf19hN/S2F&*(GHJYT*&^JaS5bGe8Rnso4CNEsCltPyV7+
AWS_DEFAULT_REGION=us-east-1
AWS_BUCKET=jetshow-public-dev
```

11. Test email via password reset
12. Test file upload via user profile pic
13. Test 2fa by enabling and logging out/in with your phone

# Set up queue and cache and sanity test

