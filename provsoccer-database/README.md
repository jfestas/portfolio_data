# Sports Agency Database Platform (ProvSoccer Lda)

**Commercial project**: Full-stack CRM platform for **football agency operations** - player/team management, scouting and deal tracking (2025).

## Core Entities (PostgreSQL)
PLAYERS (tblPlayer)
├─ Personal info, stats, reports, contracts
├─ Multiple nationalities, positions
├─ Agent assignment + contacts
└─ Performance grades + notes

TEAMS (tblTeam)
├─ League/country hierarchy
├─ Scouting needs (positions, salary limits)
├─ Team representatives/contacts
└─ Youth academy flag

OPERATION HISTORY AND MANAGEMENT
├─ Apresentações (tblPresentation)
├─ Negociações (tblNegotiation)
├─ Contratos (tblContract)
└─ TeamNeedPlayer matching

## Technical Implementation

**Backend**: pandas + SQLAlchemy/psycopg2
**Database**: PostgreSQL with indexes + foreign keys  
**Frontend**: Tkinter desktop app for data entry/visualization
**Features**: Multi-user, search/filter, export CSV/Excel

## Tech Stack
Python | PostgreSQL | Tkinter | SQLAlchemy/psycopg2 | pandas

## Schema Highlights
- **Normalized design** with referential integrity
- **Complex relationships** (player-position, team-need-player)
- **Enums** for foot, presentation/negotiation types
- **Full audit trails** (created_at/updated_at)

**Production platform** managing 100+ players, active negotiations.
