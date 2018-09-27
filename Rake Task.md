1. Rake utility allows you to create a job/task which uses rails environment. 
2. Rake tasks that allow you to perform database migrations, generate Rails scaffold files, etc.
3. By default,rakefile is come while installing the rails.

**GETTING A LIST OF RAKE TASKS AVAILABLE IN PROJECT**

rake -T


**RUN THE RAKE TASK AVAILABLE IN PROJECT**

rake namespace:task

**EXAMPLE:**
```ruby
namespace :temp
desc "TEST"
task replace_mfn: :environment do
  print "testing the rake is working or not"
end
```

Rake task will save into lib < tasks < temp.rake

**Note:** Namespace name file name will be same.

**RUN THE RAKE TASK WITH ENVIRONMENT IN WHICH ENVIRONMENT IT IS WORKING-DEVELOPMENT/PRODUCTION**

rvmsudo RAILS_ENV=development rake temp:replace_mfn
