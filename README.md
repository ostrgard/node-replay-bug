Steps to reproduce
----------------
1. Delete recorded fixtures (if any)
2. `nvm use 8` (or however you manage node versions)
3. `REPLAY=record npm start`
4. Note that fixtures are recorded for all three fetching methods on both https and http.
5. Delete recorded fixtures
6. `nvm use 9.0.0`
7. `REPLAY=record npm start`
8. Note that fixtures are recorded for all three http fetching method, but only `https.get` fixtures for https requests.