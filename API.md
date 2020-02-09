# getting auth token

`curl -v https://bilety.kkm.krakow.pl/api/v1/auth/login --data '{"email":"...","password":"..."}' --header "Content-Type:application/json"`

`{"authToken":"...","expireTimeUtc":"2020-02-09T22:43:21.9160011Z","partner":false}`

# getting all tickets data

`curl -v https://bilety.kkm.krakow.pl/api/v1/tickets/list --header 'AuthToken:...' --header 'X-Device-Id: anything'`

`{"tickets":[{"id":...,"ticketGuid":"...","status":"active","kind":"normal","type":"network_first_zone","datePurchase":"2020-02-09T21:13:22.9953274Z","startDate":"2020-02-09T23:00:00Z","endDate":"2020-03-09T22:59:59Z","monthsPeriod":1,"daysPeriod":7,"price":69.0000,"isAnyAssigned":true,"assigned":false,"canAssign":true,"forCitizen":true,"lines":[]}],"code":null,"message":null}`



