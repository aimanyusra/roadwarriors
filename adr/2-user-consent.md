# Requiring Users to Provide Consent For Third Party Access to Travel Data

## Status

Accepted

## Context

Since users are only able to sync their travel data manually, it is important for them to provide consent for third parties to access their travel data. This is so we can provide the users a better experience with real-time travel updates on their reservations.

## Driving Decisions

1. Updates coming directly from our third party partners can be considered the most accurate and on-time as opposed to waiting for updates via emails
2. This is also we can comply with regulations such as GDPR and allows us to be transparent with the usage of the users’ reservations data

## Decision

- We are not getting updates from users’ emails, we are getting them directly from the Third Party Integrations (SABER, APOLLO, travel agencies)
- Users are required to accept the terms & conditions on the system to provide 3rd party services (SABER, APOLLO) details of their reservations upon sync/create
    - This is to allow real-time updates for changes in their reservations

## Consequences

1. Might turn away users whom are concerned about privacy
2. If by any chance the user’s booking isn’t supported by our third party partners, they will not be able to receive real-time updates
