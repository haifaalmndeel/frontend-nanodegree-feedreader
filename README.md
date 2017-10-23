
# frontend nanodegree feedreader

#####  __First__ thing to do is that I have to Write a test that loops through each feed in the allFeeds object and ensures it has a URL defined and that the URL is not empty. 
* I write a loop for` URL defined` and `name defined` to check if it defined and not empty 

#####  __scond__ write a new test suite named `The menu`
* Write a test that ensures the menu element is hidden by default. You'll have to analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
  * I write a a test expect menuIcon to equal false because in the code menuIcon    should retune fulse bu default.

* Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: does the menu display when clicked and does it hide when clicked again.
    * I write a a test expect menuIcon to have been called after you cLick on the menu 

##### __thirdly__ write a new test suite named `Initial Entries`
* Write a test that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container.
   * first I write beforeEach function for loadFeed to make sure its called first because its asynchronous
   * second write test expect loadFeed to have been called

##### __Fourthly__ Write a new test suite named `New Feed Selection`
* Write a test that ensures when a new feed is loaded by the loadFeed function that the content actually changes.
   * first I write beforeEach function for loadFeed to make sure its called first because its asynchronous
   * second write test expect allFeeds not to equal loadFeed
