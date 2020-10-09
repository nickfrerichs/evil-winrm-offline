Steps used to bundle gem files

https://stackoverflow.com/questions/4402819/download-all-gems-dependencies

gem install bundle

Getting Gem with Dependencies:

    Create a new Folder with a File named Gemfile in it.
    Write a Source and the Gem you want to have the dependencys for into the File
    Bsp:

        source "http://rubygems.org"
        gem 'rails', '3.2.1'

    Open a Commandline at this Folder an Execute: bundle install
    This should download and install all Dependencys
    Execute the Command bundle list if you wanna see it
    Execute the Command bundle package
    This should create the Directory Structure vendor/cache
    Inside the cache Directory are now all the Dependencys you need for your gem

Install Gem on Machine without internet connection:

    Copy the cache Folder to the Machine
    Open a Commandline inside the Cache Folder and execute gem install --local Gemname.gem
    Bsp:

        gem install --local rails-3.2.1.gem


