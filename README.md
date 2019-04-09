# compare_grades
Let's compare climbing grades I guess

For those of you that don't know me: I like to rock climb, eat ice cream, and make self depricating jokes. I want to get less fat, so I decided I would eat less Ice Cream. I also want to climb harder. Thus a rule: I woul only eat ice cream if I sent 5.13a or harder. I then made the rules a little bit more structured. The ice cream trip is at the end of a weekend or day (if I'm local). So everything  ends up on the same cone, if I somehow manage to climb more than one 13 in a weekend (or my life god). Here are the cone and topping rules:

|Grade   |Reward   |
|--------|---------|
|5.13a   |Standard Cone   |
|5.13b   |Waffle Cone   |
|5.13c   |Waffle Cone dipped in fudge   |
|5.13d   |Waffle Cone Dipped in fudge + fudge on top of ice cream   |

The rules are kinda flexible, if I'm at a shope w/o special waffle cones I just get fudge on the ice cream, or whatever.

Anyway, I'm starting to get into bouldering this year, and want to carry my ice cream rules over. It seemed like there was a lot of debate about VX == 5.Y. So, I did what any wanna be smart kid would do, turned to 8a.nu and wrote some shitty code. We're half way there. To compare the different grades I scrapped the top 1500 sport climbers and boulderers world wide. This was low-key a bit of a pain because you have to use Selenium and Beautiful Soup. Then I threw it all into plotly and boom! an ok graph that you can mouse over.

Then I got curious (read: bored) and decided I would try to add a line with the BMI for sport climbers and boulderers onto the graph. This looked like it would be easy enough, I already had their names and just had to throw the names(replacing the ' ' with a '-') into a url and scrape the table. It obviously couldn't be that easy and was actually kind of a pain. By which I mean it took like 3 hours to get running. You have to send 8a a user-agent to access user profiles (I guess?) and I found one that apparently mimics the chrome one (I guess?). I also had to clean out non-ascii characters, whcich was also a pain. I ended up just kinda not worrying about names with Unicode-8+ characters. If you'd like to add that functionality, please send me a pull request. Getting this data after I got the code working took like 3 hours on a mid-grade computer with a terrible internet connection, plus the 8a servers aren't really that fast.

Anyway. I'm adding the BMI Lines now and might try to figure out how to add more mouse over text to the chart in a while. But then again, maybe I won't who knows what will happen next in the boring life of Mason Caiby?
