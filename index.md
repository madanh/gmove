## GMOVE — a Google maps feature that could relief the climate crisis

Hennadii Madan

Google’s mission is to organize the world’s information. This noble activity has already changed the world in more than one way. Now, when humanity is facing the climate crisis — the biggest challenge in it’s existence, it is exhilarating to discover that Google has unique power to dramatically and rapidly reduce global CO2 emissions and change the fate of humanity, by “purely software means”. Unlike other “green technologies”, there’s no need to wait 10–15–30 years to see the effects, but will start having impact as soon as it is implemented (could be within a year).

The information that needs to be organized this time is “who is going where (and wants to help with climate crisis)”. And the means to achieve this organization is by adding a single feature to Maps, a product already deployed on billions on smartphones worldwide.

# Description

The following user story illustrates the core functionality.

### Jane:

I live in the suburbs in place A. I’m about to drive to a place B downtown that I haven’t been to before. I’m going to drive alone and have three empty seats. I open google maps on my mobile, search for place B. I habitually select drive option (although a new ‘gmove’ option is presented as default). On the bottom of the screen directions appear, besides direction two new checkboxes appear (selected by default). One says ‘pick up up to 3 passengers‘ and has controls near 3 that enable adjusting this. The other says ‘allow detours up to 1 km’ with similar controls.

I don’t change anything and tap ‘Start’.
https://miro.medium.com/max/700/1*rRI5mTUYDszrBVmjpagL5Q.png


### Joe:
I live in the suburbs in place C, within 300m of route from A to B. I plan my drive to place B while sitting on a couch at home. I notice that the new ‘gmove’ means of transportation is present (and selected by default). The icon has a little red circle with number 1. This number is the number of drivers that are willing and able to take me to within 500m of B. The description of the route says “ Gmove –share a ride” and has walking instructions to a point D where I can be safely picked up by Jane. It also hase Jane’s ETA at D and walking instructions from C to D. I leave my car keys on the table, tap start and go to D.

https://miro.medium.com/max/700/1*rzj9Ub_ZwcmjGfH2lKL3TA.png

### Jane:

3 minutes before I would have approached D I receive a notification that Joe will wait for me there, and that we will prevent 4.2 kg of CO2 from being emitted. Driving instructions changed so that I can pick up Joe at D. I follow the instructions.

### Joe:
I follow the walking instructions and arrive at D 5 minutes before Jane’s ETA. My phone’s screen now has a QR code that will allow Jane to know that I’m indeed her passenger (in case there happens to be more than one Joe at D).

### Jane:
I follow the instructions and pull over at D. I scan Joe’s QR code and we are both congratulated by our phones and encouraged to proceed with out common trip. Joe occupies the passenger seat and buckles up. Driving instructions resume and I continue driving. We have a hilarious chat with Joe about this new feature and how awesome and easy it is. We wonder how Google makes it work. Finally we arrive at B. The phone says “You have arrived at your destination AND prevented 4.2kg of carbon dioxide emissions. Way to go!” Joe thanks me , I thank him, and we part ways with a feeling of connection to humanity.

Other user stories are possible, but this would make this document too long.

You can use the [editor on GitHub](https://github.com/madanh/gmove/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

# How much Global CO2 emissions may be prevented
## Best case scenario (upper bound)

I know that this is hyper optimistic, but let’s just dream about what could happen. Not immediately, but eventually if we not only provide the means to fill up those empty cars, but also invest into changing the culture. Let’s dream BIG!
Definition

### Let’s define the best case scenario:
I. A cultural shift is induced and enabled by ‘gmove’. People give priority to this transportation option over driving, taking taxi, Uber or bus.

II. The cultural shift is adopted so well, that people who otherwise would consider buying a car, choose to rely on ‘gmove’.

III. Gpackage (see Additional Features) is adopted.

### Upper bound estimation
I.

Let’s assume that all drivers adopt this and fill their free seats with other drivers. This means that the average car occupancy goes to 4.0 from the current number but the same number of users use less cars.

So, current number of cars in the world is estimated at

Nc=1.42*10⁹ .

Current average car occupancy in UK (https://www.statista.com/statistics/314719) is

Ac = 1.55.

If we extrapolate this to the world, then the total number of car users is

Uc = Nc*Ac = 2.2*10⁹.

Now let say that gmove + promotion campaign leads to a new car occupancy

An = 4.0

Then the new number of cars needed to transport Uc users is

Nn = Uc/An=0.55*10⁹.

By this estimate gmove would remove

Dcars = Nn-Nc = 1.65*10⁹

cars from active usage. Average annual CO2 emissions of a typical vehicle are estimated at

F= 4.6*10³ kg.

This leads to the net prevented CO2 emissions from part I of best case scenario of:

Di = F*Dcars = 7.59 10¹² kg = 7.59 Gt CO2

This amounts to 19.2% of 2018 global emissions estimate, and is taken from the “transportation” emission source.

II.

Around 50% of CO2 emissions associated with a car happen during it’s manufacture. If gmove removes demand for 1.65*10⁹ new cars, this means that another

Dii = Di = 7.59 Gt CO2

would stay in the form of unburnt fossil fuel. This part of saving would come from the “industry” emission source.

III.

I don’t quantify this contribution because it would be a fraction of the remaining emissions from transportation and would be negligible compared to I and II
# Additional features

This list is nowhere near being exhaustive and is just something that I actually bothered to write down.

## Total CO2 prevented
Keep an account of total CO2 emissions prevented by all users and display it when . This might incentivize some users. It also adds a base for future rewards programs.

## Gpackage
Driver is given an option to pick and deliver a package along his course. This one is tricky, since it implies monetary incentives and a separate UI for the package sender. Monetary incentive is quite dangerous, since it may dramatically change the behavior and lead to reduced adoption not only of gpackage but also gmove.

# Credit
Original idea belongs to Marko Cafnik, who sought to build a monile app implementing a platform for low-latency ride sharing and ad-hoc package delivery. I, Hennadii Madan, figured that it would take ages to for that app to come into use and it would be much better for the humanity if Google were to implement it in Maps.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List


**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/madanh/gmove/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
