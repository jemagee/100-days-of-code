# 100 Days Of Code - Log

### Day 5: August 12, 2017

**Today's Progress**: Worked on the recipe application on the ingredient side.  Completed the basic CRUD with testing, established a root (not a big deal) but found how to test that a root route goes to the right place.  I had never done that before.  A little more styling, and use of font-awesome.  Though not directly coding, also set up the OSB project on my computer, which actually took a long time to get to work on test recordings.  

**Thoughts**:  Nothing really new today, the work with OBS that I finally got working did make me think about maybe doing a test recording.  We'll see how that goes.  Perhaps an 'introduction/getting started' thing.  As for a future direction on the project, I could continue to flesh out the basics or move to the has many through and it's complication which will force javascript to be used and tested in the UI, or could work on styling more, with a navbar, those always take me too long.

**Link to work**: [Recipe Project](https://github.com/jemagee/recipes)

**Links Used for Today's Work**

* [Relish for Rspec Help](https://relishapp.com/rspec/rspec-rails/v/2-3/docs/routing-specs/route-to-matcher)
* [Font Awesome](http://fontawesome.io)
* [OBS Project](https://obsproject.com/)

### Day 4: August 11, 2017

**Today's Progress**: Worked on the recipes a bit more today, implementing an edit function, refactoring the form as I like to do (including different custom go buttons), and refactoring the errors to a shared element that takes *object* so that it can be used for all forms.  Did some more styling.  Finally took a serious look at font-awesome, turns out there's a better way to implement it into buttons and it's hella easier to style that way.  

**Thoughts**:  Friday's are going to be short, at least I got an hour in right?  Working on CSS styling is still a fight to be at least content with how something looks.  Seems that Bootstrap 4 is now *official*, the standard getbootstrap web site goes to a page that is new today.  While I primary prefer Reddit these days to find answers for my own questions, it seems that stack overflow is still the primary repository for solutions to previously asked questions, according to web search engines.

**Link to work**: [Recipe Project](https://github.com/jemagee/recipes)

**Links Used for Today's Work**

* [Bootstrap](http://getbootstrap.com) (with a note, seems BS 4 might be official, so if you're still using 3 be careful)
* [Font Awesome](http://fontawesome.io)
* [Stack Overflow Answer on FA](https://stackoverflow.com/questions/33662623/rails-using-font-awesome-icons)


### Day 3: August 10, 2017

**Today's Progress**: I started a new project, that I've always wanted to do because I think it's a good portfolio project that can force a lot of skills to be learned.  It's a recipe application, which I know is boring, but I haven't really seen one I like (baking is ratios, but recipes don't have *parts* in them usually).  

**Thoughts**:  In three days, I've worked on three different projects, I realized today that having a variety of projects will not only help me not get **stagnant**, but might help me focus on different things.  For instance, I did some (basic) styling on the recipe application today.  Integrating javascript with my applications, along with front end design, have always been issues for me and I think the other projects might force me to develop other muscles simultaneously.  Hopefully, I can work on each project at least one day a week, but that depends on inspiration and development. I even wrote some tests that would take into account proper styling appearance because it's relatively new to me.

**Link to work**: [Recipe Project](https://github.com/jemagee/recipes)

**Links Used for Today's Work**

* [Bootstrap](http://getbootstrap.com)
* [Rails API guide for content_tag](http://api.rubyonrails.org/classes/ActionView/Helpers/TagHelper.html#method-i-content_tag)

### Day 2: August 9, 2017

**Today's Progress**: I have a very old project that got unwieldy and messy so I decided the best way to do it would be to start it over.  It was initially built as company specific, but hopefully (even with amazon purchase) it can become more useful.  Participated in the Code Newbie weekly twitter chat (it's an hour and I only have 2 free hours a night, so to me it counts because it motivates me).  Did a brief sketch of the models and how they might interact and how some are indepdent from the others.  

**Thoughts**:  Much like getting back into testing yesterday, the new application creation needed a refresher (I forgot -T cause I prefer RSpec and I prefer to start with postgres, just easier that way), plus installing the gems I want and getting even the basics going took some reminding.  I feel that resetting this project makes sense not only because I want to make it more accessible to many users (companies) at the beginning, but I can re-model somethings, and I can (hopefully) work on some layout stuff in the future.  Hopefully my new model layout will reduce some of the repetition an allow for more useful data to be extracted from the whole foods raw data.  Starting over a project that I know the direction of is also helpful is reanimating the muscles that have atrophied a bit as well as building on new skills at the same time.

**Link to work**: [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

**Links Used for Today's Work**

* [RSpec-Rails](https://github.com/rspec/rspec-rails)
* [CodeNewbie on Twitter](https://twitter.com/codenewbies) (some jagoff has used codenewbie and never tweeted, twitter squatters - who knew)
* [Shoulda Matchers](https://github.com/thoughtbot/shoulda-matchers)

***Things I want to work on Next***

* Applying validations and error control to the company creation, smoothing out the layout for errors and flash to have some style using bootstrap
* Adding a logo uploading feature (with tests) for the company
* Working out the brand concept - one company can have multiple brands that might have a unique UPC prefix - maybe brand isn't the right word, but figuring out a way to extract the UPC Prefix into its own model would save time when auto creating individual item information

### Day 1: August 8, 2017

**Today's Progress**: Started basics of creating a user profile on Code Connection, including adding the first user specific trait, country.  

**Thoughts:** It's incredible how fast the programming muscles can atrophy - it's been a while since I've written any rails code (a coupld months) let alone any serious code at all (a few weeks) due to a variety of reasons, but I am going to have to get back into this project to get it to work.  It's obviously a much bigger project than I could have possibly thought but if I don't do work on it no one else is going to.  Hopefully I'll get faster and more focused as time goes on.  I also used a new gem, country_select, and found that stack overflow is still the primary source of archived answers to problems, even though I prefer reddit for current discussions.

**Link to work:** [Code Connectino](https://github.com/jemagee/code_connection)

**Links Used for Today's Work**

* [Country Select Gem](https://github.com/stefanpenner/country_select)
* [Countries Gem](https://github.com/jemagee/code_connection/projects)
* [Selecting A Value from a list, using Capybara](https://stackoverflow.com/questions/25282012/selecting-value-in-dropdown-with-capybara)

***Things I want to work on Next***

* I'd like to make the users/id path so it just shows profile, thought I figured out how from the rails guide, but did not.
* The profile information needs to expand, time zones are helpful, some countries have many, it'd be nice to link the time zone to the country so if it's only one it's automatically populated but if country has many the select list only has those options - yay Javascript or VueJS?
* There are over 500 countries in the country_select, being able to start typing the name of your country to narrow down the list would be nice, selectize is a nice JS tool for that, but implementing js testing in RSpec can be tricky
* Layouts Layouts Layouts, I didn't really do any styling of layouts, just put the information on the page required for tests to pass

