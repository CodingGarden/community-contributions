Intro to Redux with React 16  
======

View the video [here](https://www.youtube.com/watch?v=_l8z3TTlQQo)  

## Important Links  

* [Github repository for the video](https://github.com/CodingGarden/intro-redux)  
* [Redux Website](https://redux.js.org)  
* [Yarn's Documentation](https://yarnpkg.com/en/docs)  

## Suggested Videos  
  * Prerequisites - The Following Coding Garden Videos:  
    * [What Is Application State](https://www.youtube.com/watch?v=7ilYJAG-_Ug)  
    * [State Management and Component Hierarchy -Vue.js-](https://www.youtube.com/watch?v=lRE03MBZnuY)  
    * [Intro To React](https://www.youtube.com/watch?v=vIA130MePY8)  

## Outline  

* [1:23] Show start / Introduction  
* [1:55] Overview of Project  
* [2:38] Prerequisites -Videos listed above- (Have an idea of what state is and be familiar with React)  
* [3:56] What Is Redux and Where To Find More Info About Redux  
* [4:30] What is application state?  
* [6:36] Back To Redux  
* [6:43] Redux Diagram/Flow  
    * [7:05] Store  
    * [7:40] Provider  
    * [7:53] Container Components  
    * [8:09] Presentational Components  
    * [8:35] Action Creators  
    * [8:44] Actions  
    * [9:09] Reducers  
* [10:53] Container Components Revisited  
  * connect  
    * mapStateToProps  
    * mapDispatchToProps  
* [11:56] Another Redux Diagram/Flow (animated)  

* [12:29] Convert a Simple Todo React app to Redux  
  * [12:42] Create A Copy Of no-redux Named with-redux for comparisons afterwards 
    * [13:11] Snags A Beverage! Nice!  
    * [13:32] Welcome Back  
    * [14:06] Is Redux Used With Non-React Apps? (Chat Question)  

  * [14:49] Quick Tour Of The App - Pre-Redux  
    * [17:38] Is Redux Similar To Vuex? (Chat Question)  

  * [18:22] Start Adding Redux React-Redux Redux-Logger  
    * [18:40] yarn add redux react-redux redux-logger  
  * [18:58] Create a basic store  
      * [19:08] state  
      * [20:10] reducer  
      * [20:59] export reducer  
  * [21:17] Render App with Provider wrapper and store  
  * [23:08] Connect container to the store  
    * [23:47] mapStateToProps  
    * [25:11] Convert to use props instead of state  
  * [25:40] Checking Progress And Fixing Errors  
  * Convert method calls to dispatch calls  
    * Starting With newTodoChanged  
    * [28:01] Convert change handlers to action types and reducers  
      * [28:30] action types  
      * [29:09] actions  
      * [30:08] reducer  
      * [32:05] mapDispatchToProps  
      * [32:51] Converting newTodoChanged  
        * [34:10] Move TodoApp Component Into A Folder Called Containers  
        * [34:46] Update To Reflect The File Move  
      * [35:09] Finish Converting newTodoChanged Into A Dispatch Call  
  * [36:50] Observe App Using redux-logger  
  * [39:10] Observe App Using Redux Dev-Tools  
  * Continuing To Convert Method Calls To Dispatch Calls And Change Handlers To Action Types And Reducers  
    * Creating addTodo And Changing formSubmitted  
      * [42:10] Create Action Type ADD_TODO  
      * [42:28] Add addTodo To The Actions  
      * [42:42] Update Reducer for when ADD_TODO Is Called  
      * [43:28] Bring The Action To mapDispatchToProps  
      * [43:50] Call New addTodo Action Inside formSubmitted  
      * [45:00] Observe And Debug All The Changes  
    * Converting toggleTodoDone  
      * [48:18] Create Action Type TOGGLE_TODO_DONE  
      * [48:48] Updating The Action For toggleTodoDone  
      * [49:18] Update The Reducer For toggleTodoDone  
      * [50:35] Bring The Changes To mapDispatchToProps  
      * [51:35] Call The New toggleTodoDone Action  
      * [52:52] Observe And Debug All The Changes  
    * Converting removeTodo  
      * [54:04] Create Action Type REMOVE_TODO  
      * [54:15] Updating The Action For removeTodo  
      * [54:30] Update The Reducer For removeTodo  
      * [55:31] Call The New removeTodo Action  
      * [55:48] Bring The Changes To mapDispatchToProps  
      * [56:13] Observe All The Changes  
    * Converting allDone  
      * [56:54] Create Action Type ALL_DONE  
      * [57:17] Update The Action  
      * [57:40] Update The Reducer  
      * [58:22] Bring The Changes To mapDispatchToProps
      * [58:41] Call The New allDone Action  
      * [58:55] Observe All The Changes  
  * [59:55] Compare The Two Todo Apps With And Without Redux  

* [1:02:48] Talking About API Calls And Async Actions  

* [1:04:47] Convert a Simple Image Search React app to Redux (API calls)  
  * [If You're Curious About How The App Was Built](https://youtu.be/qQGPpUmDSPI?t=2573)  
  * [1:07:31] Preping Project: Copying All Needed Items - Installing Packages  
  * [1:08:40] Start Converting To Redux  
    * [1:09:23] Create Store  
    * [1:09:47] Create Reducer  
    * [1:10:46] Create Provider  
    * [1:11:19] Hook Up Store To The Component - mapStateToProps  
    * [1:11:39] mapStateToProps  
    * [1:12:53] Observe Changes In Browser  
    * Convert searchTermChanged  
      * [1:13:10] Create Action Type SEARCH_TERM_CHANGED  
      * [1:13:21] Create Actions  
      * [1:13:47] Update Reducer  
      * [1:14:28] mapDispatchToProps  
      * [1:15:51] Call The Converted searchTermChanged Action  
    * [1:16:16] Add In A logger With redux-logger  
    * Create setLoading  
      * [1:17:58] Create Action SET_LOADING  
      * [1:18:28] Update Reducer  
      * [1:18:52] Update mapDispatchToProps  
      * [1:19:12] Call The New setLoading Action  
    * [1:19:30] Add an async action middleware  
    * [1:19:43] redux-promise-middleware setup  
      * [1:22:56] Create getImages  
      * [1:23:22] Grab The API  
      * [1:23:59] Talking About How To Handle The Images  
      * [1:24:30] Update Reducer To Handle The Images  
      * [1:24:58] mapDispatchToProps getImages  
      * [1:25:25] Call The Newly Created getImages Action  
      * [1:25:52] Observe And Debug All Changes  
      * [1:26:34] Handle The Images In The Reducer  
      * [1:27:20] Observe Changes  
    * [1:28:43] Refactor  
    * [1:31:13] redux-thunk: Viewing Documentation And Explaining  
    * [1:32:54] View A More Complex Redux App (campsite-list inside github repo)  
      * [1:33:05] no-redux Version Of App  
      * [1:34:13] with-redux Version Of App  
* [1:37:42] Closing Thoughts  
  * [1:40:45] Outro  

Contributed by: @zeroIndex0
