# stuff
Going to keep some stuff here

## jq
Print raw lines, but pprint json:
curl -is "https://api.open-meteo.com/v1/forecast?latitude=52&longitude=13&current=temperature" | jq -Rr '. as $raw | try fromjson catch $raw'

