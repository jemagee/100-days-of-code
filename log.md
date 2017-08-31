# 100 Days Of Code - Log

### Day 17: August 30, 2017 (It's a Wednesday)

**Todays Progress**:  Got some general *model* planning done on paper.  It's a start.  The application like I said is going to be query heavy.  Once it's set up, only one table changes much.  It's probably a warehouse but I don't know NoSQL yet so it's staying in PostGres.  Finished up the basic first model set up and testing.  Layouts can wait until later.  Starter the second step model which is connected to the first.  Participated in the CodeNewbies Twitter chat, which I did say to myself I wasn't going to do.

**Thoughts**:  This heat wave in california is obnoxious, it's 8:30 and i'm sweating as I type, it is not condusive to studying or focusing.  Air conditioning would be so great, and maybe I'd get more done in my limited time.  Even this log got the short shrift today cause it's freaking hot and I need to turn off all heat sources I can.

### Day 16: August 29, 2017.

**Today's Progress**: Sometimes you have to take a step back to take a step forward.  The Whole Foods Project I was building is too complicated to start with.  Assumes a lot of things that I don't know yet.  I do know how to build a basic database for my company that I work at now as I already have one, so I decided to start a second whole foods project, scaled down, for one company only.  It's easier to conceptualize from the beginning and if the application expands it is expandable to a multi-company design if needed.  Set up the application with my standard gems, and started with the first model, basic, one attribute to work with.

**Thoughts**: I'm going to try and plan this out a bit better.  The hardest part, long term, aside from just laying it out in a way that is pleasant to look at will be the complex queries.  They are stable and have been used in SQL Server for probably close to a decade, but automating things always makes things more complicated.  Building the queries will probably be the last step, first need to work through the basic model creation and then the data upload.

### Day 15 1/2:  August 28, 2017

**Today's Progress**:  Doing a little research and studying today.  Trying to figure out the best way to plan a project so that it isn't *overplanned* but I don't box myself into a corner where I realize I done messed up a long time ago and am better off starting over than stepping back.  I also reviewed an older youtube video I've seen before regarding a different way to add related records within rails.  I'm not 100% sure how using the standard `has_many` / `belongs_to` with the nested form is better, and no one else seems to be able to help.  I also found a few articles trying to help you **plan** bettr via Dev.to - not sure how much help they'll be. *(side note: does anyone remember the old days when titles were capitalized except for the basic to/the/of type words?)*

**Resource Links for Today**:

[Pragmatic Video on Comments, AJAX](https://www.youtube.com/watch?v=K-sns5tNdTY)
[Plan All of the Things](https://dev.to/jlhcoder/plan-all-of-the-things)
[Yes! You Can Plan Your Projects](https://dev.to/mistermocha/yes-you-can-plan-your-projects)
### Day 15: August 27, 2017

**Today's Progress**:  Today was more of a working on new stuff day.  I tweaked my code from last night due to someone answering my reddit question with an obvious answer that hadn't occured to me.  Then I went back to working with *accepts_nested_attributes_for*, working through it from the beginning with notes this time, then moving on to cocoon, and then working through the adding from the show view, via javascript/AJAX.  It's rough of course, but it works.  

**Thoughts**: Implementing AJAX/JS responses is still a bit hard for me, I did get it done but it wasn't instinctive.  Going back over something I just learned and learning it again I think is a good step, it reinforces, and each time I write it a bit more on my own.  I consider *learning days* when you're as limited in time as me as valid parts of the 100 days even if it's not primarily the qualification.  I gotta change the qualifications :)  I also need to start learning how to **plan** projects better.  Not just the idea, but how will the idea be achieved, what does it need.  Since I don't always do that I run into conflicts, or not knowing what to do next, or parts that don't fit together properly.  Due to napping sick people, I had to limit my tutorials to words, not audio, today.  My own office would be super, but who has the room :)

**Resource Links for Today**:
* [Sitepoint on ANAF & Cocoon](https://www.sitepoint.com/better-nested-attributes-in-rails-with-the-cocoon-gem/)
* [SO Q&A on emptying a form, using trigger](https://stackoverflow.com/questions/6653556/jquery-javascript-function-to-clear-all-the-fields-of-a-form)
* [jQuery API on Append](http://api.jquery.com/append/#append-content-content)
* [My Reddit Question on Planning](https://www.reddit.com/r/learnprogramming/comments/6wdshs/planning_your_projects_out/)

### Day 14: August 26, 2017

**Today's Progress**:  Continued working on building up recipe components with ingredients.  Created conditonal destroy function so an ingredient can not be destroyed if used in recipes, in a clean manner.  (Rails prevents the delete but throw and unpleasant error if you try).  Worked on some styling of Ingredients (with testing) to display them with recipes they are used in.  Using what I learned experiementing previously on day 13, I allowed the component addition on the show page as well.  I still had to refer to the notes from the previous day, but it was better.  Properly tested and set up dependent destroy on the recipe components relationship to avoid the error that is inherent if you don't.  Set up conditional method within the ingredient model that will only pull not already assigned ingredients when working with a recipe.

**Thoughts**:  Friday August 25, no coding was done.  Ironically I did have the day off *real job*, but so did my wife, and since she works 3:30 to midnight, we don't see each other much during the week, so I think that's a god reason to have skipped a day.  Hope to make up time over the weekend with multiple hours, as many *Saturday chores* were also done on Friday.  Sometimes tricky things show up, like if you use related records, your basic destroy function becomes more complicated.  It will throw a rails error by default if you haven't set up an allow destroy and sometimes you can't.  

**Link to Work**: [Recipe Project](https://github.com/jemagee/recipes)

**Resource Links for Today**:

* [ARQ Rails Guide](http://guides.rubyonrails.org/active_record_querying.html)
* [SO Post for Querying Arrays](https://stackoverflow.com/questions/6900297/rails-where-sql-query-on-array)

### Day 13 3/4: August 24, 2017

**Today's Progress**:  Using my previous study of accepts_nested_attributes_for, I started working on adding specific ingredients to recipes (as components) for my recipe application.  I worked on some display as well, laying it out.  Using the fractional gem to allow decimal conversion.  Of course it was all tested as well.  Though not code related, worked a bit on the video work to try and get screens a bit more readable and fitting on the youtube.  Needs more practice before getting started it seems.  

**Thoughts**:  I like fractions, it took me a moment to find the gem I had used in the past (fractional) but it still seems to work, though it needs some attention since FixNum is deprecated in ruby 2.4.  I created [an issue](https://github.com/thechrisoshow/fractional/issues/8) about it - but the gem seems a bit neglected - and I don't know how to do it - perhaps I'll try.  I am using decimals as inputs because recipes should be scalable - if my recipe is for a dozen but you want to make 18 - it should scale it's own way, no?  Or if it's a baking recipe (using parts), it should perhaps convert to weights, we'll see.  This is only day 13 3/4 because I was going back and forth between coding and NFL preseason Eagles game...I didn't shut out distractions. 

**Link to Work**: [Recipe Project](https://github.com/jemagee/recipes)

**Resource Links for Today**:

* [SO on Decimals in rails forms](https://stackoverflow.com/questions/18898947/rails-number-field-alternative-for-decimal-values)
* [Fractional Gem](https://github.com/thechrisoshow/fractional)

### Day 13 1/2: August 23, 2017

**Today's Progress**:  It's Wednesday and I partook in the [codenewbie](https://www.codenewbie.org/) weekly Twitter chat.  It's an hour, so that's why today is a half day.  I consider it progress to partake in it as *people who code* are not really a part of my every day life.  I started sketching out notes for my new blog project in an attempt to plan something in advance.  At least an outline of things, so that I have a plan. 

**Thoughts**:  The blog might be my video project so I can't really start on it just yet.  It might be the topic of the videos and as such should wait.  I disovered that the video I uploaded is too small to see on youtube (the text and such) so I have to figure out how to work on the resolution (imac retina display source) so that things are visible - if people can't see what I'm writing it will sort of only be half arsed.  Requesting input from people online doesn't seem to be helping too much so I'm just going to have to decide what direction I want to go myself I guess.



### Day 13: August 22, 2017

**Today's Progress**:  Following up on more *nested attribute* work, I was able to use my lunch break to actually take another step forward.  Implemented a new *demo app* for nested attributes playing on my laptop this time but also implemented Cocoon.  Worked through a glitch on the edit function that doesn't show up on on the new function, depending on your set up (include the child id in the parent params.require function).  Used my new found knowledge of basic nested_attributes to try and put nested attributes on a show page, with tests, got it to work with some struggle.  I wanted my nested attribute to have a customer flash mesage if it succeeded and using the rails routes guide, I seemed to get it to work.  Then I wanted to be tricky and carry the nested errors back to the form - that required some modification of the show form as when you use render the built nested object is brought back with a id.nil

**Thoughts**: Chris from [GoRails](http://www.gorails.com) not only makes great videos but he's a great guy and quick twitter answer...if you aren't using his videos and following him on twitter, catch up folks.  Still thinking about the video plan, I want to maybe build something from scratch that might be of interest to people (who might also want to contribute).  At the moment deciding between recipe type site or blog.  Assuming nested attriutes would be straight forward on show page was silly, but SO did come to the rescue, though had to reduce my test because of flash message.  But then I thought, I can build my own method to handle this as this is a special action.  It was pretty easy to get the 'success' working, but getting the errors for the realted message to come back was cool.  Though I've been doing code most of the days so far, I've been rehashing ideas I've done before and getting the muscles working.  This is the first *new idea* I've handled in a long time - very happy about it.  

**Link to Work**:

**Resource Links for Today**:

* [Sitepoint how-to on ANAF and Cocoon basics](https://www.sitepoint.com/better-nested-attributes-in-rails-with-the-cocoon-gem/)
* [GoRails](http://www.gorails.com)
* [GoRails on Twitter](https://twitter.com/excid3)
* [SO on Nested Attributes on Show Page](https://stackoverflow.com/questions/17146285/fields-for-in-the-show-view-nested-attributes)
* [Member Route Addition](http://guides.rubyonrails.org/routing.html#adding-more-restful-actions)

### Day 12:  August 21, 2017

**Today's Progress**: If you could call it progress.  Once again NBA.com has gone and changed their website in a way that breaks my application from crawling through some of their information as it was previously.  Spent some time working with their new page to try and find a way to access the information I need, but as of yet have not found it.  To compound the frustrating day, I attempted to learn something new I should have worked on a long time ago, nested attributes in forms.  Should have been easy but made it difficult.

**Thoughts**:  Finding good introduction how-to and why documentation isn't easy, plus, in the case of *accepts_nested_attributes_for* there are multiple ways (optional: true, inverse_of: parent) to solve the same issue.  Yet no one clearly expalins the difference.  That's not a terrible thing, but is frustrating, oh well.  I was able to finally claw together a basic nested_form but seems all the good stuff you would want to use nested forms for actually is quite difficult to accomplish in rails so I'll have to either use a Gem (Cocoon) or get deeper into Vue.js via GoRails Tutorial

No work to link to - just wrote a tiny app to futz around with the nested_form code...one of those slower days where I had to take my limited time to try and learn something, and the time I thought I was going to work on learning was actually taken up by something else at lunch.  Better luck tomorrow I guess.


### Day 11: August 20, 2017

**Today's Progress**: Moved forward on some more individual set up on the whole foods project, adding items through the brand item, but still very simply.  Completed the brand CRUD work and got started on items.  

**Thoughts**:  It's probably about time to start working with *accepts_nested_attributes* in Rails.  I've never really dealt with it before, but I probably should.  There's so much inter-mingling within the database that adding a related record should be easy.  Using JavaScript would make it easier but it does seem kind of involved in addition.  Thinking I might start BLog 2.0 as the project for the screencasts.  We'll see.

**Link to work**: 

* [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

### Day 10: August 19, 2017

**Today's Progress**:  Worked on adding brands to the whole foods application, related to the company, with some validations I haven't worked for before (must be a six digit integer for a specific attribute).  Recorded my *pilot* video for perhaps doing youtube videos.  

**Thoughts**:  It took more time than I thought just to get the video right.  Thought OBS would be able to merge videos, seems not, and working with iMovie for the first time wasn't as easy as I had hoped but it is free.  Also working out the range thing was nice, hadn't used that one before that I can recall.  (Opressive heat makes one tired when they don't have A/C).  Friday was the culmination of a rather exhuasting (in every way) week at work combined with getting home later than normal, so I just had to take an off day. 

**Link to work**: 

* [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)
* [Youtube Video](https://www.youtube.com/watch?v=GQkhO0ARDQw)

**Links used for today's work**

* [shoulda-matchers homepage](https://github.com/thoughtbot/shoulda-matchers)
* [rails validation guide](http://guides.rubyonrails.org/active_record_validations.html)

### Day 9 1/2: August 17, 2017

**Today's Progress**:  Minimal progress in re-familiarizing myself with an application that I've been neglecting for a while due to stuckness.  Spent time working on SQL queries using PGAdmin to reacquaint myself with the database tables and the types of information I might want to have.

**Thoughts**: Though I worked for an hour on what I did today, I'm calling it a half day because, well, the SQL queries I was writing weren't that useful and I struggled quite a bit at the beginning since I haven't worked with the database or postgres for a while, so working out the kinks was a bit fun.  It was productive in that it stretched a dormant / atrophied muscle, but still not enough for me to call it a *full day* of the 100 days.  Oh yeah, the microphone came.

**Link to Work** [nba project](https://github.com/jemagee/nba) - no added work today but feel free to look at the schema and tests 

This is a fun query I played with:

```
Select p.fname,  p.lname
		,SUM(threesmade) * 100 /SUM(threestaken) * 1.0 AS "reb"
from players p 
inner join statistics s
on p.id = s.player_id
group by p.id
having 
avg(s.time_played) > 1200
AND
count(s.*) > (Select count(distinct gamedate)/5 from games)
AND avg(threestaken) > 3
ORDER BY reb DESC
```
This query takes a total of 423 players and isolates the 210 who meet the qualifications I have come up with to determine 'qualification' in terms of appearances to be a league leader.  For the longest time I kept getting a divided by zero error and thinking it was an integer problem, but the issue was that I wasn't taking into account that some qualified players might not take any threes, so I had to come up with an average to work with as well (3 is low I think) to eliminate all the zeroes.

Now - how do I convert this into AR language?  I don't know (I've turned the qualification into a method to isolate player IDs but that might not be the way to go)

**Links used for Today's Work**

* [PGAdmin](https://www.pgadmin.org/) - I didn't really use this link - but it's a handy app if you wanna write queries for your PG databases before trying to figure out how to get them into a rails application.  The above query is pretty simple as it only takes into account two tables really - if I want to do splits based on home and away or against certain divisional opponents, there's a lot more joins and qualifications require.

### Day 9: August 16, 2017

**Today's Progress**:  Worked on editing and *destroying* a store, which I set up traditionally, but then altered as I don't want stores to be destroyed so much as just 'closed'.  I then implemented a javascript solution so that you see the change on the page, which in general is pretty straight forward in Rails.  **However**, setting up testing to work with Javascript is not so straight forward in Rails and I had to find the right post (below) to get it set up properly.  This is not something I fully understand so much as just know how to get going.

**Thoughts**: Someone who works on rails, please, setup a simpler way to get testing to work with javascript, setting it up is a bear and honestly, if it weren't for my dedication to trying to built thoroughly tested applications, I probably would not test any Javascript actions at all...wow, what a pain.  Again allowed myself to be distracted by twitter, so my hour was a minimal hour and took longer than it should have.  I need a thorough complete way to block things (including whole applications) when I'm coding.  Hey Focus seemed like a good idea, but not so much and the application withered on the vine it seems.  On hey, my microphone is coming tomorrow. And I realized I've been working on the same application for many days in a row, but if the microphone works, I can start working on another application.

**Link to work**: [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

**Links Used for Today's Work**

* [Setting Up appliction to do JS testing with RSpec/Capybara](https://www.devmynd.com/blog/setting-up-rspec-and-capybara-in-rails-5-for-testing/)
* [GoRails Video on Rails UJS/AJAX](https://gorails.com/episodes/jquery-ujs-and-ajax)
* [Speech from American President - I watch it a lot](https://www.youtube.com/watch?v=OC2jhQ0KAAU)

### Day 8: August 15, 2017

**Today's Progress**: Finished up the creation of a new store within the whole foods application and testing it for the various errors possible in setting up a new store.  Used the *internationalization* to do some minor tweaks to how things might be displayed so they were more user friendly.  Started working on the editing of stores (and thorough testing) as well, but that's still a work in progress.

**Thoughts**: Using the internationalization aspect of Rails to make things more friendly is a bit annoying...in ruby one of the things I love is white space doesn't matter (yeah I'm looking at you python) but it very much matters within these files and did cause me an issue for a while, though a bigger issue I'm still having troubl with is how to deal with not propoerly selecting from a drop down list to choose the related record the new record *belongs to*.  Must exist is an awful default error code.  I also realized I can probably use this for my form buttons instead of manually changing them to Add and Update all the time...Also, annoying days at work lead to less focus but at least I got it done today.  Also while watching a GoRails episode today, I saw that his scaffold used *.update* instead of *.update_attributes*, and I kind of new the latter had been deprecated but hadn't really sussed out for waht, until now.

**Link to work**: [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

**Links Used for Today's Work**

* [SO Answer that pointed me to the Rails Guide below](https://stackoverflow.com/questions/808547/fully-custom-validation-error-message-with-rails)
* [Rails Guide on il8n](http://guides.rubyonrails.org/i18n.html)
* [Reddit Question I submitted on error customization issue](https://www.reddit.com/r/rails/comments/6tyzuf/custom_error_message_question/)


### Day 7: August 14, 2017

**Today's Progress**: Moved forward with the whole foods project, created the region model and basic testing, wrote all the creating in one sitting instead of one step at a time, model testing and then feature form testing, all done in the span of one pomodoro so that's nice.  Worked on getting started with store addition, first model related to another model, ran into some hiccups on using the select, but at least solved those.

**Thoughts**:  Still getting the eyes back in the realm of computers at work and at home, probably could work another 20 minutes or so but resting my eyes seems better.  Dealing with needing regions for store creation, instead of seeding the proper regions I just used factory girl to create a few and when I finally figured ou the select list properly, I was able to select the right one.  Hopefully it'll stick around this time so I won't have to look it up.  Still going to do basic CRUD going forward, but maybe writing the test all out at once, then working through the steps, including Model validation.  Gets done faster and hopefully more smoothly at the same time.

**Link to work**: [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

**Links Used for Today's Work**

* [Rails Guide on Form Helpers](http://guides.rubyonrails.org/form_helpers.html)
* [Rails Guide on Validations](http://guides.rubyonrails.org/active_record_validations.html)
* [Rails API Guide on Collection_Select](http://api.rubyonrails.org/classes/ActionView/Helpers/FormOptionsHelper.html#method-i-collection_select)

### Day 6: August 13, 2017

**Today's Progress**: Finished up the basic functionality of adding a company within the whole foods project, testing included.  Sketching out other models that are required and working on testing ideas for them.  

**Thoughts**:  I know I'm probably over testing and repeating things, but reinforcing the foundation of CRUD creation (and testing) even with a single attribute is helpful to making it second nature, before I get into the more advanced interactions on most of these projects, I should be sure to be fluent.  More screencast thinking and microphone exploring.  Woke up with what turned out to be a giant migraine that sadly lasted half the day so it limited my output today sadly.  Hopefully keep it up next week though...lunch and dinner.

**Link to work**: [Whole Foods Project](https://github.com/jemagee/WholeFoodsProject)

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

**Link to work:** [Code Connection](https://github.com/jemagee/code_connection)

**Links Used for Today's Work**

* [Country Select Gem](https://github.com/stefanpenner/country_select)
* [Countries Gem](https://github.com/jemagee/code_connection/projects)
* [Selecting A Value from a list, using Capybara](https://stackoverflow.com/questions/25282012/selecting-value-in-dropdown-with-capybara)

***Things I want to work on Next***

* I'd like to make the users/id path so it just shows profile, thought I figured out how from the rails guide, but did not.
* The profile information needs to expand, time zones are helpful, some countries have many, it'd be nice to link the time zone to the country so if it's only one it's automatically populated but if country has many the select list only has those options - yay Javascript or VueJS?
* There are over 500 countries in the country_select, being able to start typing the name of your country to narrow down the list would be nice, selectize is a nice JS tool for that, but implementing js testing in RSpec can be tricky
* Layouts Layouts Layouts, I didn't really do any styling of layouts, just put the information on the page required for tests to pass

