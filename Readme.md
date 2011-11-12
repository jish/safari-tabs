Safari Tabs

I wanted to switch to Safari for a while to benefit from their html5 support
and smooth animations, etc. However, when I switched, I ran into nothing but
pain. I guess I never realized how much I relied on ⌘1, ⌘2, ⌘3, etc... for
tab navigation.

While trying out Safari, I was constantly pressing ⌘1, ⌘2, ⌘3 and Safari kept
navigating to apple.com, yahoo.com, and the like -- losing whatever was in my
current tab.

Frustrated by the experience, and still inclined to give Safari a try, I dove
into the world of Applescripts to fix this little problem.

I'm no Applescript expert, so the contents of these scripts are heavily
borrowed from random sites I found while Google'ing around looking for
answers. Unfortunately during my Google Driven Development phase, I wasn't
interested in writing down every single url I stumbled upon -- and let's be
honest, they're only like 5 lines long...

On my journey to reclaim ⌘1, I really wanted to find a native way to map
keyboard shortcuts to Applescripts, unfortunately, that is easier said than
done, and it seems everyone out there writing applescripts is using some
third party application to map their keyboard shortcuts. Although, if you
know of a way to do this, please let me know!

The one I -- and many others -- have settled upon is FastScripts
http://www.red-sweater.com/fastscripts/. Don't worry, it's free for the first
10 keyboard shortcuts, and I only mapped ⌘1-5, so you'll still have 5 more
shortcuts available.

Installation

The Applescripts
* clone the repository
* rake install

Keyboard shortcuts
* Install FastScripts http://www.red-sweater.com/fastscripts/
* Open FastScripts
* Go to Script Shortcuts
* Expand /Users/<username>/Library/Scripts > Applications > Safari
* Map ⌘1-5 to the scripts titled tab1-5 respectively

Enjoy Safari's html5 support and rendering engine without wanting to kill
someone.
