# Privacy Policy — Personal Health MCP

_Last updated: 2026-08-25_

This policy describes how **Personal Health MCP** ("the Software") handles data.
The Software is a private, single-user tool run by its own author on their own
computer. It is not a product, not a service, and has no users other than the
person who installed it.

## What the Software is

The Software is a set of locally-run programs that authenticate to the WHOOP API
using OAuth 2.0 and retrieve **the authenticating user's own WHOOP data on their
own behalf**. It runs entirely on the user's personal macOS machine. There is no
server, no hosted component, no account system, and no other user.

## Data the Software accesses

With the scopes granted during WHOOP authorization, the Software reads the
authenticating user's own:

- Basic profile (`read:profile`)
- Body measurements (`read:body_measurement`)
- Physiological cycles and strain (`read:cycles`)
- Recovery scores (`read:recovery`)
- Sleep activities (`read:sleep`)
- Workouts (`read:workout`)

All requests are **read-only**. The Software cannot and does not create, modify,
or delete anything in the user's WHOOP account.

The Software does not access, and cannot access, any other person's WHOOP data.

## How data is handled

- Data flows directly between the user's own computer and WHOOP's servers over
  HTTPS. It is **not** transmitted to, collected by, or stored on any server
  operated by the author or any third party.
- Retrieved data is stored in a local SQLite database file on the user's own
  computer, readable only by that user's macOS account.
- OAuth access and refresh tokens are stored in the user's **macOS Keychain**.
  They are never transmitted anywhere except to WHOOP's own token endpoint.
- There is no analytics, no telemetry, no crash reporting, no advertising
  identifier, and no third-party data sharing of any kind.
- Nothing is sold, licensed, published, or shared with anyone.

## Other data sources

Alongside WHOOP data, the Software may store on the same local machine:

- Apple Health / Apple Watch data, exported by the user from their own iPhone.
- The user's own Microsoft 365 calendar metadata, used to compare meeting load
  against recovery trends.

This data is likewise stored only locally and is never combined with, uploaded
to, or disclosed to any external service. WHOOP data is never sent to Microsoft,
Apple, or any other party.

## Retention and deletion

The user controls retention entirely. Deleting the local database file removes all
stored data permanently. WHOOP access can be revoked at any time from the WHOOP
mobile app, or by deleting the OAuth grant, after which the Software can no longer
retrieve any data.

## Children

The Software is used solely by its adult author and is not directed at or made
available to children.

## Third-party services

The Software communicates with the WHOOP API. Use of WHOOP and of WHOOP data
remains governed by WHOOP's own privacy policy and terms, available at
<https://www.whoop.com/legal/>.

## Changes to this policy

Any change will be reflected in the "last updated" date above.

## Contact

Enquiries regarding this policy may be directed to the email address registered
with the associated WHOOP developer application.
