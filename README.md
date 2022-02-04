# Mushroom Festival
Use [this template](https://github.com/alchemycodelab/half-baked-web-01-mushroom-festival) to get started.

# Plan
I) Display mushrooms and friends on load
    A) Display mushrooms    CHECK
        1) Clear mushroom div   CHECK
        2) Loop through and add a mushroom for every iteration for mushroom count   CHECK
    B) Display friends  CHECK
        1) Clear out friends    CHECK
        2) Feed friend object into displayFriend (creates html from object) CHECK
        3) Add event listener to friend, on click
            a) if mushroom left and friend less than satisfied  CHECK
            b) decrement mushroom   update state    CHECK
            c) increment satisfaction   update state    CHECK
            d) display friends  update DOM  CHECK
            e) display mushrooms    update DOM  CHECK
            f) If satisfied, no more mushroom   CHECK
            g) If no mushroom, alert to forage  CHECK
        4) Append friends to DOM CHECK
II) Invite creates and displays new unsatisfied friend CHECK
    A) add event listener to adding friend  CHECK
    B) on submit    CHECK
        1) create new friend object CHECK
            a) with given name or random CHECK
            b) with random satisfaction CHECK
        2) pass new friend object to display friends function   CHECK
III) Forage adds more mushroom is successful
    A) Event listener
    B) On click
        1) Check if mushroom found
        2) Alert if found
        3) display mushrooms
IV) Friend click disappears mushroom and satisfies friend
    1) Taken care of in friend event listener
V) If friend is satisfied, no more mushroom, if feed friend and no mushrooms get more
    2) Taken care of in friend event listener

## Learning Objectives

-   In response to a user event, mutate a single object in a state array and display the new state to the user (i.e., complete a todo).
-   Describe the difference between a pure and impure function.

### Live Example:

https://alchemycodelab.github.io/web-01-mushroom-festival/

# Acceptance Criteria

-   User should see some mushrooms and default friends on load
-   Click on the 'invite' button to create a new (unsatisfied) friend (with a random default name if none is provided) and add them to the page
-   The number of mushrooms should be visible on the table and should update when mushroom state changes.
-   Clicking the forage button should launch an alert telling the user if they found a mushroom. 50% of the time, the user should succeed.
-   On clicking a friend, a mushroom should vanish from the table, and the friend should become more satisfied. Satisfaction level should be visible to the user as different emojis
-   On clicking a friend, if that friend is completely satisfied, they can eat no more mushrooms. Also, if you try to feed a friend and there are no mushrooms, user should get an alert telling them to go forage for another mushroom.

# Mushroom Festival

| Deploy Requirements                                   |     |
| ----------------------------------------------------- | --- |
| Main branch deployed to Netlify                       | 1   |
| Open PR from `dev` branch with Netlify deploy preview | 1   |

| Requirements                                                        |     |
| :------------------------------------------------------------------ | --: |
| addFriendButton event listener adds new unsatisfied friend          |   2 |
| displayFriends function displays all friends and adds click handler |   2 |
| displayMushrooms displays the mushrooms                             |   2 |
| when page loads users see default friends and mushrooms             |   2 |
