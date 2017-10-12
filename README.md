[![Build Status](https://travis-ci.org/mini-kep/db.svg?branch=master)](https://travis-ci.org/mini-kep/db)
[![Assertible status](https://assertible.com/apis/56e34b07-ae3a-4248-937e-fef69d8ec2f2/status?api_token=VkiQoHOdjWU3vGv2)](https://assertible.com/dashboard#/services/56e34b07-ae3a-4248-937e-fef69d8ec2f2/results)

## Specification

- <https://github.com/mini-kep/intro/blob/master/specification/database.md>

## Sample GET calls 

#### ```names```:
- [api/names/a](https://minikep-db.herokuapp.com/api/names/a)
- [api/names/q](https://minikep-db.herokuapp.com/api/names/q)
- [api/names/m](https://minikep-db.herokuapp.com/api/names/m)
- [api/names/d](https://minikep-db.herokuapp.com/api/names/d)

#### ```datapoints```:
- [api/datapoints?name=CPI_rog&freq=m](https://minikep-db.herokuapp.com/api/datapoints?name=CPI_rog&freq=m)
- [api/datapoints?name=GDP_yoy&freq=q](https://minikep-db.herokuapp.com/api/datapoints?name=GDP_yoy&freq=q)
- [api/datapoints?name=BRENT&freq=d&start_date=2017-01-01](https://minikep-db.herokuapp.com/api/datapoints?name=BRENT&freq=d&start_date=2017-01-01)
- [api/datapoints?name=USDRUR_CB&freq=d&start_date=2017-08-01&end_date=2017-10-01](https://minikep-db.herokuapp.com/api/datapoints?name=USDRUR_CB&freq=d&start_date=2017-08-01&end_date=2017-10-01)

Errors:
- [wrong freq](https://minikep-db.herokuapp.com/api/datapoints?name=ABC&freq=z&format=json)
- [wrong name for such freq](https://minikep-db.herokuapp.com/api/datapoints?name=ABC&freq=q&format=json)
- [start date in future](https://minikep-db.herokuapp.com/api/datapoints?name=BRENT&freq=d&start_date=2025-01-01)
- [end date > start date](https://minikep-db.herokuapp.com/api/datapoints?name=BRENT&freq=d&start_date=2015-01-01&end_date=2000-01-01)


#### ```info```:
- [api/info?name=CPI_rog&freq=m](https://minikep-db.herokuapp.com/api/info?name=CPI_rog&freq=m)
- [api/info?name=GDP_yoy&freq=q](https://minikep-db.herokuapp.com/api/info?name=GDP_yoy&freq=q)
- [api/info?name=BRENT&freq=d](https://minikep-db.herokuapp.com/api/info?name=BRENT&freq=d)
- [api/info?name=USDRUR_CB&freq=d](https://minikep-db.herokuapp.com/api/info?name=USDRUR_CB&freq=d)

More methods [discussed here](https://github.com/mini-kep/db/issues/8#issuecomment-336152762).

