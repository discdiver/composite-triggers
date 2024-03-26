# Composite triggers

## Compound & sequential triggers: what's the difference?

A compound trigger is a trigger that is activated by multiple events. For example, a trigger that is activated when a player enters a certain area and presses a button. A sequential trigger is a trigger that is activated by multiple events in a specific order. For example, a trigger that is activated when a player presses a button and then enters a certain area.

## How to implement them?

See the [docs](https://docs.prefect.io/latest/concepts/automations), Guidry made some great examples and explanations.

## Problem 1: Basic compound trigger

1. Make an automation with a trigger that fires when two different events occur in any specified order and within 2 minutes of each other.
1. Make the automation action to send an email.
1. Test it manually.

## Problem 2: Basic sequential trigger

1. Make an automation with a trigger that fires when two different events occur, but only in the specified order and within any time frame.
1. Make the automation action to send an email.
1. Test it manually.

## Problem 3: Compound trigger in event-driven workflow with custom payload -> deployment parameter

Note: work here is ongoing and may need to build from Main.

1. Make an automation with a trigger that fires when two out of three custom events or webhook hits occur within three minutes of each other.
1. Make sure one of the custom events has a custom payload.
1. Run a deployment for the automation action.
1. Use the payload from the custom event as a parameter value for the deployment.
1. Test it manually.
