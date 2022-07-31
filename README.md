# Python and Accessibility

## Origin Story

As I was experimenting on myself with radiation therapy... hmm, too far back, let's jump ahead.
This repo started as a place for me to create a talk, titled "Python and Accessibility," for
[PyBay2022 - Food Truck Edition](https://pybay).

I've never given a conference talk but am optimistic I'll enjoy the experience.
And maybe this initial talk, intended to be 10 minutes, can grow into something more technical with greater depth.
If the talk does go well, and I continue wanting to present accessibility to Python developers, I'll add to this repo.

### Proposal for the Talk

Here is what I submitted as the talk proposal.  It serves as the jumping off point and the theme of this repo.

<quote>
As Python becomes a realistic option for web, mobile, and cross-platform  application development, Python developers need to, at the very least, have an appreciation and high level understanding of accessibility.

<a href="https://pyscript.net/"> __PyScript__ </a> has the potential to introduce Python as a first class option for developing web based applications.  It promotes the ability to draw from component libraries to quickly create fully functional web apps.  If those components are not developed with an understanding of accessibility though, we will continue to experience inaccessibility and alienation of many users.

<a href="https://beeware.org/"> __BeeWare__ </a> is a set of tools enabling a Python developer to deploy their single Python code base as applications across many different platforms.  And the apps will use components native to each platform.  By using platform native components, accessibility is more likely, but not at all guaranteed. 

The creators and developers of BeeWare and PyScript surely understand and appreciate accessibility and will do what can be done in their technologies to encourage it.  Frameworks and toolkits though cannot be too strict thus much of the responsibility for accessibility will rest on the app developers.

I'd like to spend 10 minutes introducing accessibility and why it matters and why Python developers should understand and embrace it.  It's unlikely I will get into any code details given the time, though I do expect it to be a technical talk.  My goal is to plant the seed and advocate for a deeper understanding of accessibility within the Python community.
</quote>

## Introduction

What is __accessibility__ (often abbreviated as __a11y__) and why does it matter to Python developers?

### Accessibility

At a high level, I think of accessibility as __understanding and appreciating who your users are, how they might interact with your product based on their current abilities, then using that understanding to guide the user experience design and user interface development__.

Perhaps some of your users have low or no vision, or are temporarily in a situation where they cannot see the screen.
Or perhaps they don't hear well, or at all, or are in some environment where sound would be inappropriate.
Or maybe they have temporary or permanent mobility issues and are not able to press small, close together buttons on a touch screen.
Or are dealing with cognitive challenges and are overwhelmed by a very busy and crowded screen.
or, and And I suspect this resonates with the developers here, you don't want to have to take your hands off the keyboard to use a mouse.
Many people are dealing, to some degree, with a combination of the situations listed above.

There are existing technologies, standards, and guidelines for developing usable applications to people in these temporary or permanent situations in life.
For web content, though some of the standards are applied more broadly to applications in general, there's an amazing amount of information at the
[Web Accessibility Initiative (WAI)](https://www.w3.org/WAI/).
To get started, there's a collection of introductory information on the WAI site at
[Accessibility Fundamentals](https://www.w3.org/WAI/fundamentals/).

You might have heard of ,
[Web Content Accessibility Guidelines (WCAG2)](https://www.w3.org/WAI/standards-guidelines/wcag/) and
[Accessible Rich Internet Applications (ARIA)](https://www.w3.org/WAI/standards-guidelines/aria/).
Those are important of course, but hardly the complete picture.
For a list of standards and guidelines, including links to current versions, drafts of new iterations, and brief summaries, see
[W3C Accessibility Standards Overview](https://www.w3.org/WAI/standards-guidelines/).

```<rant>```
One standard I don't think gets enough focus is the
[Authoring Tool Accessibility Guidelines  (ATAG)](https://www.w3.org/WAI/standards-guidelines/atag/).
The point of the ATAG is tools intended to be used by others to develop web content not only need to be accessible themselves, they need to generate content that is also accessible.
So many times I have gone to a small company site and its accessibility is marginal at best, even for mostly static content.
I look at the source for the page and it's so full of divs and spans and random looking ids, it must have been generated by some tool.
If the ATAG were taken more seriously by companies focused on enabling small businesses to setup an online presence, it would be a nice boost to overall accessibility of eCommerce.
```</rant>```

### What Does This Have To Do With Python Developers?

In the [results for the PSF and JetBrains 2021 survey of Python developers](https://lp.jetbrains.com/python-developers-survey-2021/),
Python does not score highly for developing desktop or mobile apps.
It does score highly for web development though.
However, 69%  of Python web developers also use JavaScript and 60% use HTML and CSS.
I think it's safe to say Python is used on the backend while JavaScript/HTML/CSS are used to generate the UI.
That's hardly a revelation to any Python developers reading this.

#### Python Is Making Its Move

As noted already, Python is venturing not only in to web front end development with PyScript, but becoming a viable option for cross platform desktop and mobile with BeeWare.
Maybe it seems Python is a bit late to the game, JavaScript has existed for decades, dominates the web frontend, and, with electron, is a viable option for the desktop.

PyScript and BeeWare are not trying to break in to an industry with mature tooling and libraries and frameworks used by most developers.
They are entering domains in flux with what appears to be infinite patience for ditching older ideas for new possibilities.

### Wrap It Up

There seems to be plenty of room and time for Python to disrupt web, desktop and mobile apps.
And unfortunately, the bar for accessibility has been set fairly low across those domains.
Python developers have a great opportunity to show the world how intuitive, and accessible, a user experience can be.
