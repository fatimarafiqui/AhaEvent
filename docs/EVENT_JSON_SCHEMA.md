# Event JSON Schema

```
{
    "EVENT_ID": {
        "eId": EVENT_ID,
        "name": EVENT_NAME,
        "timestamp": {
            "start": START_DATE_TIMESTAMP,
            "end": END_DATE_TIMESTAMP
        },
        "location": LOCATION_NAME,
        "geolocation": {
            "longitude": LONGITUDE,
            "latitude": LATITUDE
        },
        "links": {
            "website": WEBSITE_URL,
            "register": REGISTRATION_URL,
            "logo": LOGO_URL,
            "coverImg": COVER_IMG_URL
        },
        "cfp": {
            "timestamp": {
                "start": CFP_START_TIMESTAMP,
                "end": CFP_END_TIMESTAMP
            },
            "link": CALL_FOR_PROPOSAL_URL
        }
    }
}
```

### About Keys Used in the above Schema

| Key                   | Mandatory | Description | Example |
|-----------------------|-----------|-------------|---------|
| EVENT_ID              | Yes       | Unique event ID | See Below |
| EVENT_NAME            | Yes       | Name of the event in English | Open Source Summit 2018                                                                  |
| START_DATE_TIMESTAMP  | Yes       | Timestamp of the day and time at which the event starts.| 1529433000000 for 20th June 2018 |
| END_DATE_TIMESTAMP    | Yes       | Timestamp of the day and time at which the event ends.| 1529433000000 for 20th June 2018 |
| LOCATION_NAME         | Yes       | Location where the event is going to take place.| Tokyo Conference Center Ariake, Tokyo, Japan |
| LONGITUDE/LATITUDE    | Yes       | Longitude/Latitude of the location. In case the coordinates are not available, city coordinates can be provided.| 139.6917 / 35.6895 |
| WEBSITE_URL           | Yes       | Complete website link of the event| https://events.linuxfoundation.org/events/open-source-summit-japan-2018/ |
| REGISTRATION_URL      | Yes       | Complete event registration link| https://events.linuxfoundation.org/events/open-source-summit-japan-2018/attend/register/ |
| LOGO_URL              | Yes       | Complete link of the event's logo. If not available, logo of the organization can be used. | https://events.linuxfoundation.org/wp-content/uploads/2017/11/logo_ossummit_jp.png |
| COVER_IMG_URL         | Yes       | A cover image to show on event card. It can be an image of the event or the city hosting it. | https://events.linuxfoundation.org/wp-content/uploads/2017/11/tokyo-2.jpg |
| CFP_START_TIMESTAMP   | Yes       | Timestamp at which the call for proposals will open.| 1529433000000 for 20th June 2018 |
| CFP_END_TIMESTAMP     | Yes       | Timestamp at which the call for proposals will close.| 1529433000000 for 20th June 2018 |
| CALL_FOR_PROPOSAL_URL | Yes       | Complete link to the call for proposal landing page.| https://events.linuxfoundation.org/events/open-source-summit-japan-2018/program/cfp/ |


### Event ID

Currently EVENT_ID is just URL_SLUG.

| Key                   | Mandatory | Description | Example |
|-----------------------|-----------|-------------|---------|
| URL_SLUG              | Yes       | URL slug for the event. It should meet the following conditions: i) All characters must be small ii) It should include event name, city and year only. iii) Space can be replaced by a dash ( '-' ) only. | open-source-summit-tokyo-2018 |
