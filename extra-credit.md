#### Search History
---
- Dedicate a section of your page to show a list of all previous search queries made in the current browser.  Title this section **Search History**.
  - This list should only display searches made using the current browser.  
  - Since we do not have a concept of _Logging In_, the search list should be tied to the browser, not a User.
- When a new search is submitted, it should automatically appear in the **Search History** list.
- When a **Search History** item is clicked, the same search should be conducted.
- The search history should be persistent. Use either [Firebase](https://www.firebase.com), or an API on your Server to read/write the info to a database or a file.
  - Again, the search history must be specific to an individual browser.  This means using two separate browsers should yield two separate search histories.
  - Upon closing and re-opening the browser, the search history should be retained.  To accomplish this, you are expected to read the search history from your API, or from Firebase.  Since your API will support multiple search histories for various visitors, you should think of a way to uniquely identify browsers, and use this id to identify specific histories.

#### Search Auto-Complete
---
- Using the User's search history, make the search box an auto-complete box that will suggest recent searches based on what the User is typing.
 - An example of an auto-complete box can be found under the *typeahead* section on the following page:
   - https://angular-ui.github.io/bootstrap/#/typeahead

#### Grading
---
Search History
- **20pts** - Display Search History unique to the browser.  If it is not unique to the browser, you will not receive credit.
- **10pts** - Make each Search History item clickable so that when clicked, the search is repeated.
- **20pts** - Persist and read the history using an API (either Firebase or an API that you created).

Search Auto-Complete

- **25pts** - Display auto-complete suggestions as the User types.
- **25pts** - Use the unique search history that is tied to the browser.

#### Total: 100pts

###Due by December 7th, 2015 at 11:59PM.