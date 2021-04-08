# Code 401 Class 38 Reading Notes

## How granular should your reducers be
* Single-responsibility can be beneficial for reducers, however, there are times when granularity is beneficial. It depends on how many aspects of state need to be changed in a given action
* [Source React Kung Fu](https://reactkungfu.com/2016/11/how-granular-are-your-redux-actions/)

## Pro or Con - multiple reducers can "fire" when a commonly named action is dispatched
* Having multiple reducers fire for a commonly named action can be beneficial to aid in dry code but can also result in confusion and bugs if not handled correctly. Another issue can occur if you are trying to change state at the same time in two different places.
* [Source Redux.ruanyifeng](https://redux.ruanyifeng.com/faq/Actions.html#should-i-dispatch-multiple-actions-in-a-row-from-one-action-creator)

## Name a strategy for preventing the above
* To prevent the above you can use thunk middleware to create a sequence of dispatching so that the state is not altered twice at the same time.
* [Source Redux.ruanyifeng](https://redux.ruanyifeng.com/faq/Actions.html#should-i-dispatch-multiple-actions-in-a-row-from-one-action-creator)

## Define the following terms
* store
  * "Store holds the state tree of your application". To be able to change it you need to dispatch actions.
  * [Source redux.js](https://redux.js.org/api/store)
* combined reducers
  * Combined reducers consists of pooling together multiple reducers in a single object for export to allow passing of the function to createStore.
  * [Source redux.js](https://redux.js.org/api/combinereducers)


[Table of Contents](README.md)