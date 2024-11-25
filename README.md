#The Yarn Shop

## An embryo of a project
A website where users can track the weaving yarns in their stash, and assign them to various projects, which should be able to calculate yarn usage. Maybe blog posts, or entries associated with users/projects.

## Features wanted
- Create user
- Update user
- Add yarn to stash
- Update stashed yarn
- Create project
- - from user page
- - from yarn page
- Add yarns to project
- Display stashed yarn on user page
- Display projects on user page
- Suggest suitable sett per yarn
- Calculate yarn usage given weaving project input

## DB tables

### User
- id
- username
- password
- displayName
- email
- yarnStash[]
- projectList[]
- blogPosts[]

### Yarn
- id
- name
- dateAdded
- datePurchased
- colourName
- colorNumber
- batchID
- vendor
- price
- skeinWeight (gram)
- skeinLength (meter)
- numberOfSkeins 
- yarnWrapsPerCM
- yarnWeight
- projectUsed
- photos[] =>
- yarnWeight (=ie NM)

### Project
- id
- name
- yarnsUsed
- calculationVariables // needs detailing
- description
- ? Blog posts about project ?
- photos[] =>

### Blog Posts
- id
- userID
- dateAdded
- lastUpdate[]
- associatedPRoject
- textEntry

photos []
- id
- userOwner
- dateAdded
- yarnID
- projectID
- blogID