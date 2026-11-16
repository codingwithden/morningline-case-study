# MorningLine: Case Study

A wake-up call service that rings your actual phone at the time you choose, landlines included.

**Status:** working prototype that places a real scheduled call. The code is private while I get it ready to sell.

## The problem

Alarms are easy to ignore. You snooze on autopilot, or you turn it off in your sleep and don't remember doing it. A phone call is different: it rings longer, a voice talks to you, and it can come from a phone across the room. Hotels have known this for years, but there's no simple wake-up call service for regular people at home.

I'm one of those people who sleeps through alarms, so I started here.

## Who it's for

- Heavy sleepers who sleep through phone alarms
- People who keep their phone out of the bedroom and use a landline or a second device
- Anyone who wants a friendlier, spoken start to the morning

## Product decisions

| Decision | Why |
| --- | --- |
| Call any phone, including landlines | The phone across the room is the whole point |
| A spoken message, not just a ring | A voice is harder to tune out than a tone |
| Pricing built from real costs | I modeled the cost of every call and every spoken message before setting prices |
| Reuse common messages | Saving and reusing popular spoken messages cuts the biggest cost and keeps plans cheap |

## Pricing

| Plan | Price |
| --- | --- |
| Free | $0 |
| Premium | $2.99 |
| Premium+ | $6.99 |

## Build plan

I broke the build into 8 steps so each one could be tested on its own. Step one was the riskiest part: can the system place a real call to a real phone on schedule? That works today. Next comes the scheduler, the voice messages, accounts and payments.

## Tech

Phone calls through Twilio, natural voice messages, a hosted database for users and schedules, and a small server that runs the scheduler.

Built by Denisse Medina Flores ([@codingwithden](https://github.com/codingwithden))
