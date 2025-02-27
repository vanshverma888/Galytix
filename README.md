# Galytix

Purpose: Calculates average GWP from CSV data.
Endpoint: POST http://localhost:9091/api/gwp/avg
Input: {"country": "ae", "lob": ["property", "transport"]}
Output: {"property": 634545022.9, "transport": 446001906.1}

Setup:
1. Requires .NET Core 3.1 SDK.
2. Run `dotnet restore` in project folder.

Run:
- `dotnet run` (starts on http://localhost:9091)
- Test via http://localhost:9091/swagger

Test Example:
- POST {"country": "ae", "lob": ["property", "transport"]}

Notes:
- Uses DI, async, error handling.
- CSV in Data/gwpByCountry.csv loads at startup.
