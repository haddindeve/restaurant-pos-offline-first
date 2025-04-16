# Offline-First Restaurant POS - architecture

A React PWA that treats the network as optional: orders are written locally first and synchronised to a Node backend when a connection exists. The kitchen and the till keep a consistent view of an order regardless of connectivity at the moment it was taken.

## Components

### PWA frontend

Order entry, table and menu management

### Local store

Offline order persistence

### Sync layer

Reconciliation with the backend on reconnect

### Node backend

Order, menu and reporting services

## Stack

| Layer | Technology |
| --- | --- |
| Frontend | React PWA |
| Backend | Node.js |
| Offline | Local-first persistence with background sync |
| Deployment | Render |

Designed and implemented by Muhammad Tanveer - Full-Stack AI Automation Engineer.