# Fetching Users’ Emails only On Demand

## Status
Accepted

## Context
One of the requirements is to allow the polling of users’ emails to retrieve latest updates related to their travel reservations. While it is ideal that our app polls them on a recurring time schedule (eg. once every 5 minutes), knowing the fact that we have 10 million total users will require a lot of resources for it to be feasible.

## Decision Drivers

1. How much resources will be needed for us to keep polling 10m users’ emails every 5 minutes feasibly?

## Decision

- Only allow users to trigger on demand
- No additional polling to user’s emails

## Consequences

1. Users are only able to create new reservations upon triggering sync
