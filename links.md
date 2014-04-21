# Links

A gathering of annotated blog posts, talks and related subjects (chronologically sorted). Start with the Introduction to Offline First by Team Hoodie:
http://blog.hood.ie/2013/11/say-hello-to-offline-first/

## Blog Posts

### Offline Support is Valuable, and You Can’t Add it Later
http://aanandprasad.com/articles/offline/ (Aanand Prasad, August 2011)

1. You can’t assume a request will complete in a short time.
2. You can’t assume a request will even make it to the server.
3. If it does, you can’t assume the response will make it back.
4. If the request does fail, you won’t know whether it made it to the server or not.
5. If the connection is slow, or flaky, it may well stay that way.

> An application designed along these traditional lines, built on the assumption that an Internet connection is not just available, but reliable and fast, will be incredibly frustrating to use over a poor-quality connection.

> Getting into the offline mindset requires only one key realisation: when you leave the world of timely, reliable communication, the local database, not the server’s, must be the gateway for all persistent changes in application state.

> When your application is designed this way, its “offline” usability skyrockets.

### Offline First – A better HTML5 User Experience
http://blog.joelambert.co.uk/2012/11/26/offline-first-a-better-html5-user-experience/ (Joe Lambert, Nov 2012)

> Offline is a feature and it’s crucial we start to consider it from the start of a project as apposed to adding support later in the development lifecycle

1. Decouple your app from the server
2. Create an API wrapper client side
3. Decouple data updates from data storage ("a Data object to act as a proxy between the API object and the rest of your app")

### Introduction to Offline First by Team Hoodie
http://blog.hood.ie/2013/11/say-hello-to-offline-first/ (Team Hoodie, Nov 2013)

> Geography is non-negotiable

> We can’t keep building apps with the desktop mindset of permanent, fast connectivity, where a temporary disconnection or slow service is regarded as a problem and communicated as an error.

see also:

- http://alistapart.com/article/application-cache-is-a-douchebag (Talk: http://www.youtube.com/watch?v=cR-TP6jOSQM)

### Will It Work If I'm Offline
http://jacobsondergaard.com/blog/will-it-work-if-i-am-offline/ (Jacob Søndergaard, Feb 2014)

see https://createlists.net/, Jacob's Offline First App.

### Do HTML5 apps have to be online all the time?
http://christianheilmann.com/2014/03/23/do-html5-apps-have-to-be-online-all-the-time/ (Christian Heilmann, March 2014)

> One would think that almost five years after the definition of HTML5 offline capabilities this question would be answered. As someone spending a lot of time on HTML5 panels and Q&A sessions at conferences I can tell you though that it gets asked every single time.

> The problem is that these are details that don’t interest the business person considering using HTML5. All they hear is experts complaining and bickering and saying that offline HTML5 doesn’t work. Which isn’t true. It doesn’t work perfectly, but nothing on the web ever does. Many, many things in Android and iOS are broken, and many apps don’t work offline either. These shortcomings are not advertised though which makes native apps appear as a much more reliable alternative. We should stop showing our behind the scenes footage as a highlight reel.

## Talks

### Building Web Apps of the future. Tomorrow, today and yesterday.
http://www.youtube.com/watch?v=O3AukCYymEU (Paul Kinlan at Full Frontal, Nov 2012)

> Oh I don't use apps on the web, I don't see the point. I just use it for news and wikipedia – Some guy

> Top 20 Apps in Apple/Android App Store, most don't need an internet connection to work. Same experiment with top 10 web apps, just don't work offline. It's a horrible experience

> Native apps completely win hands down in offline experience

> "I will add offline support into my app" – A Web Dev

> "I all add online support into my app" – An App Dev

> As web developers, we are not used to build Offline Applications. When you start, you're going to change the way you build applications.

Slides: https://speakerdeck.com/paulkinlan/building-web-apps-of-the-future-tomorrow-today-and-yesterday

### Offline Rules.
http://www.youtube.com/watch?v=RrGo1Sz4IgQ (Andrew Betts at Full Frontal, Nov 2012)

> Use AppCache for files, localStorage for settings, IndexDB for Data
> localStorage saves data with UTF-16 encoding, so you have half of the space available that you think you would


### Network connectivity: optional
https://www.youtube.com/watch?v=Z7sRMg0f5Hk (Jake Archibald at Chrome Dev Summit, 2013)

> Making Stuff work offline used to be very easy. It has only become an issue with the advent of the internet. [...] The only stream you needed from outside the building was electricity.

> These days most devices will ship with a "cache for electricity" which can be used if the stream is not available. And we call it battery.

> In the same way it makes sense to build interfaces mobile-first, it’s time to think about designing and building our applications offline-first

> Wouldn't it be great if things Wikipedia, Google Maps and Youtube would once again be resilient to fluctuations in connectivity [showing CDs of Encarta, 3D World, ...]

> Online first: Users with connectivity get fresh data all the time, users without connectivity are reused. This is graceful degradation. And as we found with graceful degradation, it's the wrong way around. [...] you cannot make assumptions on connectivity, but you do, per request, when you rely on it.

> Offline first: The next generation of progressive enhancement treats the network as a potential enhancement that might not be available.

> Sure, connectivity is getting better. But it's very rarely going to be faster than getting stuff straight off the device. This whole thing's as much about improving performance for user with connectivity, as it is for giving something to those without.

> Being predictive about the network doesn't work. navigator.onLine doesn't know anything outside your device.

> Developing for the internet has huge advantages. If a thing has a screen, it's more and more likely to have a browser on it. When someone goes down the native path and develops versions of the same thing for different languages, as a platform, we must ask why and fix that bug because it is a bug.

Slides: https://speakerdeck.com/jaffathecake/network-optional

See also:

- Notes by Luke Wroblewski: http://www.lukew.com/ff/entry.asp?1820
- ServiceWorkers explained: https://github.com/slightlyoff/ServiceWorker/blob/master/explainer.md
- ServiceWorker on GitHub: https://github.com/slightlyoff/ServiceWorker
- ServiceWorker poly fill: https://github.com/phuu/ServiceWorker-Polyfill/
- Offline Panel at Edge Conf 2013: http://www.youtube.com/watch?v=qwywMlGE0vY

### Offline first!
http://www.youtube.com/watch?v=7mdG-iAizVc (Jan Lehnardt at Realtime Conference Europe, April 2013)

> It's latency, stupid.

> Latency is more important than bandwidth. It's the important thing on the network.

> Offline = infinite latency

> Fallacies of distributed computing: 1. The Network is always fast 2. The Network is always available

> Thinking Offline First isn't better, but it enables you to build better applications

see also:

- http://writing.jan.io/2011/02/22/the-multiscreen-revolution-english-translation.html


## Related

- Automatically display online/offline indication to your users: https://github.com/hubspot/offline
- Mobile browser storage limit research: http://www.html5rocks.com/en/tutorials/offline/quota-research/
