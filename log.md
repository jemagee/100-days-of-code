# 100 Days Of Code - Log

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

