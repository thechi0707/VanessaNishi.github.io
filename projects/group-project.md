---
layout: project
type: project
image: img/group-project.logo.png
title: "Professor, I Choose You!"
date: 2024
published: true
labels:
summary: "Professor trading card website created as final project for ICS 314"
---

### Academia-Arena: A Professor Trading Card Game
For the final group project of ICS 314, my group created Academia Arena, which is a professor trading card game website. My fellow team members were Erin Patterson, Elsa Wong, Yu Fang Ma, Carlo Viloria and Michaella Villanueva. The website allows players to collect trading cards of UH Manoa ICS professors and instructors by answering computer science-related questions. The page allows them to create an account, view the cards they've collected, create a wishlist of cards they'd like to collect, pull for cards, and list cards in a marketplace for trade. Each card has the professor's name, what classes they teach and a fun fact about them. The goal of the game was to help student's learn more about their professors and encourage more interaction between CS students and their professors.

Some of our pages:
Card Pull Page (created by Michaella)
<p align="center">
<img src="../img/group-project/card-pull.png" />
</p>

Marketplace Page (created by Erin)
<p align="center">
<img src="../img/group-project/marketplace.png" />
</p>

Wishlist Page (created by Elsa)
<p align="center">
<img src="../img/group-project/wishlist.png" />
</p>

#### My Contributions
<p align="center">
<img src="../img/group-project/card-collection.png" />
</p>
For this project I was responsible for creating the Card Collection page, which lists all the cards that the user owns. This page reads from a database that holds all the cards that all users own and displays the ones that the current user owns. One of the tricker parts of this page was having different styling (color) for the cards depending on their rarity. I was able to achieve this by using an if-else statement and passing the css id names to the card component depending on the rarity. 

```
filteredCards.map((tcard) => {
    if (tcard.type === 'Common') return <Col><ThisCard key={tcard._id} card={tcard} background={commonBackground} title={commonTitle} image={commonImage} text={commonText} onTradeClick={handleTradeClick} /></Col>;
    if (tcard.type === 'Rare') return <Col><ThisCard key={tcard._id} card={tcard} background={rareBackground} title={rareTitle} image={rareImage} text={rareText} onTradeClick={handleTradeClick} /></Col>;
    return <Col><ThisCard key={tcard._id} card={tcard} background={legendaryBackground} title={legendaryTitle} image={legendaryImage} text={legendaryText} onTradeClick={handleTradeClick} /></Col>;
              })
```
I also implemented a search bar that finds cards by first or last name, added most of the professor information and adjusted the styling of the trading cards. My teammates created and sent out a form to the ICS professors, and I used the information collected from there.

#### My Takeaways from This Experience
This was the first group programming project I've done and it's taught me a lot on how to work in a team efficiently. For one, my team was really great; everyone did their part and kept things moving. We always made sure to communicate everytime we made a major commit, had any questions or needed help, etc. It was really important that we let each other know what were doing or changing, especially if it involved changing one another's code. Moreover, I learned a great group management strategy with Issue Driven Project Management. On GitHub we had Milestone projects which held all the issues/tasks that needed to be completed for the project, with three categories: To-do, In-Progress, and Done. According to the IDPM guidelines we learned, there should be at least twice the amount of to-do issues per team member and each team member should have one in-progress issue at all times. After a certain date, all to-do and in-progress issues were moved over to the next milestone, while all the done issues were preserved in the current milestone. The method of project management was great because it allowed team members to work more independently. Everyone can see clearly what everyone else is working on and once they complete a task they can simply assign themselves another one. This removes some of the hassle involved with division-of-labor and no one was left with nothing to do. We of course still had weekly meetings and talked over discord regularly, but IDPM allowed us to work more efficiently and independently. I think IDPM was one of the best takeaways from this class and is something I'd like to use for all projects moving forward, not just CS-related ones. 