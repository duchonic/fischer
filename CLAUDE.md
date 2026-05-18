# Fischer — Portugal Trip Planner

## Project overview
A single-page HTML travel guide for a Portugal hiking trip (Rota Vicentina / Fisherman's Trail), departing from Zurich.

- **Trip dates**: 22–30 May 2026
- **Route**: Faro → Sagres → Vila do Bispo → Carrapateira → Arrifana → Odeceixe → São Teotônio → Odemira → Lisbon → ZRH
- **Two files**: `travel.md` is the source of truth for bookings/logistics; `index.html` is the rendered guide.

## Workflow
When `travel.md` is updated, sync the changes into `index.html`. Key sections to keep in sync:
- Hotel booking chips (`.booking-chip`) inside each day card
- Bus/train departure times in segment metadata
- The accommodation summary grid near the top of the page (between distance bars and main itinerary)

## Accommodation summary
Located just above `<main>` in `index.html`. Shows all 8 nights with date, location, hotel name, and booked/TBD status. Update this whenever a new hotel is confirmed in `travel.md`.

## Current booking status (as of last sync)
| Night | Location | Hotel |
|---|---|---|
| Fri 22–23 May | Faro | Guest House Jacaranda Faro ✅ |
| Sat 23–24 May | Vila do Bispo | Hotel Mira Sagres ✅ |
| Sun 24–25 May | Carrapateira | Cabana 1 by Soul Houses ✅ |
| Mon 25–26 May | Arrifana | Hotel Utopia ✅ |
| Tue 26–27 May | Odeceixe | Hotel Casa Padra da Foz ✅ |
| Wed 27–28 May | São Teotônio | TBD |
| Thu 28–29 May | Odemira | TBD |
| Fri 29–30 May | Lisbon | Vista do Tejo ✅ |

## Transport bookings
- **Faro → Sagres**: Bus 10:15 → 13:17
- **Odemira → Lisbon**: Rede Expressos 048, Odemira N263, 09:55 → 12:50
- **Lisbon → ZRH**: Flight departs 13:25 on 30 May
