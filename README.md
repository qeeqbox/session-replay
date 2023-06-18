<p align="center"> <img src="https://raw.githubusercontent.com/qeeqbox/session-replay/main/session-replay.png"></p>

A threat actor may re-use a stolen or leaked session identifier to access the user's account.

## Example #1
1. Threat actor obtains a valid session identifier and does not use it immediately
2. Threat actor re-using the same session identifier to gain unauthorized access to a victim's account

## Example #2
1. Bob submits a request to buy an item from a vulnerable website
2. Threat actor finds the request and tricks bob into re-submitting it
3. The vulnerable website receives both requests with the same session identifier and processes them

## Impact
Vary

## Risk
- gain unauthorized access

## Redemption
- Identity confirmation
- Regenerate session ids at authentication
- Timeout and replace old session ids
- Store ids in HTTP cookies

## ID
fe0561ad-6ce7-4cf3-a229-eb136ad1f919

## References
- [wiki](https://en.wikipedia.org/wiki/session_fixation)
