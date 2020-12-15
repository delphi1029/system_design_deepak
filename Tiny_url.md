# Tiny Url -


URL shortening is used to create shorter aliases for long URLs. We call these shortened aliases “short links.” Users are redirected to the original URL when they hit these short links. Short links save a lot of space when displayed, printed, messaged, or tweeted. Additionally, users are less likely to mistype shorter URLs.

URL shortening is used to optimize links across devices, track individual links to analyze audience, measure ad campaigns’ performance, or hide affiliated original URLs.

## Requirements - 
Functional Requirements:

1) Given a URL, our service should generate a shorter and unique alias of it. This is called a short link. This link should be short enough to be easily copied and pasted into     applications.
2) When users access a short link, our service should redirect them to the original link.
3) Users should optionally be able to pick a custom short link for their URL.
4) Links will expire after a standard default timespan. Users should be able to specify the expiration time.

## Non-Functional Requirements:

1) The system should be highly available. This is required because, if our service is down, all the URL redirections will start failing.
2) URL redirection should happen in real-time with minimal latency.
3) Shortened links should not be guessable (not predictable).
