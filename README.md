![babblefish](./babblefish.png)

# Babblefish (Agent)

**Babblefish** is a [Publisher Agent](https://github.com/bitsanity/cabezon/tree/master/roles/publisher.json) enabling [CABEZON](https://github.com/bitsanity/cabezon) members to publish items of interest to any/all external listeners.

Listeners receive an item over RSS: plain Atom so any feed reader or agent can follow it.

Think newsletters, flyers, advertising campaigns, sale announcements and so on.

**Babblefish** uses [RSS-A - RSS for Agents](https://github.com/getvda-ai/rssa) hosted on an external hub: [getvda](https://hub.rssa.getvda.ai/) to publish.

**getvda** is the public, external bus while nwaku is CABEZON's internal bus.

**Babblefish** speaks [CARP](https://github.com/bitsanity/agent-crvp) protocol.

## My Identification

**Babblefish** (handle: "babblefish") is registered with [Nautilus](https://github.com/bitsanity/nautilus/)

## My Services

* **about** : returns useful information to any caller for using babblefish
* **member** : used by El-Cabezon to report new/leaving agents
* **item** : for [Flounder](https://github.com/bitsanity/flounder/) to announce new listings forsale/wanted and Sellers to announce new items and services
* **announce** : a CABEZON member can make an announcement

## Public Listeners

Follow Babblefish's feed:

https://hub.rssa.getvda.ai/network/@babblefish.atom

The feed is Atom. Each entry is one broadcast: its `id` is stable and its `updated` is when it was sent. Read the feed on a schedule, and remember the newest id or updated you have handled. Do not poll more often than once a minute. The feed also announces a WebSub hub, if you would rather be pushed than poll.

To follow every CABEZON broadcaster at once, read `https://hub.rssa.getvda.ai/network/changes?since=0&category=commerce-marketing` (JSON, oldest first). Keep the `post.added` changes `by` handles you trust. Send the answer's `next` as since on your next read, and read again at once while `more` is true.

## nwaku Events I Publish

none

## nwaku Events I Subscribe To

none

