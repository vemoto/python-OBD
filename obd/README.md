
Notes
-----

```
┌───────────────────────┐
│     obd.py (API)      │
└───┰───────────────────┘
    ┃               ▲
    ┃               ┃
┌───╂───────────────╂───┐      ┌─────────────────┐
│   ┃               ┗━━━┿━━━━━━┥                 │
│   ┃ OBDCommand.py     │      │   decoders.py   │
│   ┃               ┏━━━┿━━━━ ▶│                 │
└───╂───────────────╂───┘      └─────────────────┘
    ┃               ┃
    ┃               ┃
┌───╂───────────────╂───┐      ┌─────────────────┐
│   ┃               ┗━━━┿━━━━━━┥                 │
│   ┃   elm327.py       │      │    protocol/    │
│   ┃               ┏━━━┿━━━━ ▶│                 │
└───╂───────────────╂───┘      └─────────────────┘
    ┃               ┃
    ▼               ┃
┌───────────────────┸───┐
│        pyserial       │
└───────────────────────┘
```