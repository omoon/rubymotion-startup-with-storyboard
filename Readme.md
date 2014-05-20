# RubyMotion Startup with Storyboard

## What I've done

### motion create
<pre>
$ motion create xxxxx
</pre>

### Edit Gemfile
<pre>
gem 'bubble-wrap'
gem 'ib'
</pre>

### Prepare Storyboard
<pre>
$ rake ib:open
</pre>

and, add `StoryBoard` in `resources` directory.

### Edit app_delegate.rb
<pre>
@window = UIWindow.alloc.initWithFrame(UIScreen.mainScreen.bounds)
storyboard = UIStoryboard.storyboardWithName('Storyboard', bundle: nil)
@window.rootViewController = storyboard.instantiateInitialViewController
@window.makeKeyAndVisible
</pre>

## What you should do after cloning

### Edit app.name in Rakefile

### Bundle install
<pre>
$ bundle install
$ rake ib:open
$ rake
</pre>

### And more..
