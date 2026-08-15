# Real-Time Communication Research

## Purpose

Study how GoSignal can send real-time traffic-control updates from an authorized traffic controller to connected driver applications.

## Communication Requirements

The system should support:

- Real-time GO / STOP updates
- Countdown synchronization
- Route-specific updates
- Emergency alerts
- Reliable message delivery
- Low communication delay
- Connection status monitoring

## Possible Technologies

- WebSockets
- Firebase Realtime Database
- Firebase Cloud Messaging
- MQTT
- HTTPS APIs

## GoSignal Use Case

Traffic police selects a route and timing in the authorized control application.

The backend receives the command and distributes the current status to relevant driver applications.

Example:

Route A:
GO — 60 seconds

Route B:
STOP

Route C:
STOP

Route D:
STOP

## Research Questions

- Which communication method gives the lowest practical delay?
- How should countdown timers remain synchronized?
- What happens when a user temporarily loses internet connectivity?
- How should duplicate or outdated commands be handled?
- How can unauthorized users be prevented from sending traffic commands?
- How should communication logs be stored?

## Security Requirement

Only authorized traffic-control personnel and systems should be able to issue traffic-control commands.
