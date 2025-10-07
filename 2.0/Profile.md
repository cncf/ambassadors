If you need to update your [Ambassador](https://www.cncf.io/people/ambassadors/) profile, please follow the below instructions by submitting a PR for approval. After a PR is merged, the CNCF site will reflect the update within 10 min. 

For more information go to [CNCF People](https://github.com/cncf/people/blob/main/README.md).

## Listing Format

The [people.json file](https://github.com/cncf/people/blob/main/people.json) lists all people in alphabetical order by name.  Add new entries in the right place in the list.  Not all fields are used by each listing.  This is the format:

```json
    {
        "name":"Full name of person",
        "bio":"Full bio of person. Use html markup when needed.",
        "company":"Company and/or title",
        "pronouns":"Personal pronouns",
        "location":"A Google Maps readable name of city, state, country",
        "linkedin":"LinkedIn url",
        "twitter":"Twitter url",
        "github":"GitHub url",
        "wechat":"Wechat url",
        "website":"Personal website",
        "youtube":"YouTube url",
        "certdirectory":"CertDirectory.io url",
        "priority":Value to differentiate between other entries in an ordered list; omit this entry in most cases,
        "languages":[Array of languages spoken],
        "projects":[Array of CNCF projects of expertise],
        "category":[Array of categories the person belongs to],
        "email": "person!example.com",
        "slack_id": "U123ABC456",
        "image":"Image filename from the /images/ directory"
    }
```

Project names must exactly match [the landscape listing](https://landscape.cncf.io/card-mode?project=hosted).  Category names must exactly match the list above.

And here is an example entry:

```json
    {
        "name":"Johnny Appleseed",
        "bio":"John Chapman (September 26, 1774 – March 18, 1845), better known as Johnny Appleseed, was an American pioneer nurseryman who introduced apple trees to large parts of <a href='https://en.wikipedia.org/wiki/Pennsylvania'>Pennsylvania</a>, Ohio, Indiana, Illinois and Ontario, as well as the northern counties of present-day West Virginia.",
        "company":"Apples R Us",
        "pronouns":"he/him",
        "location":"Portland, Maine, United States",
        "linkedin":"https://www.linkedin.com/in/johnny-appleseed/",
        "twitter":"https://twitter.com/jappleseed",
        "github":"https://github.com/jappleseed",
        "wechat":"https://web.wechat.com/jappleseed",
        "website":"https://jappleseed.com",
        "youtube":"https://www.youtube.com/c/jappleseed",
        "certdirectory": "https://certdirectory.io/profile/4f64eb11-eeed-46ef-953a-73ecf7d561ea",
        "priority":10,
        "languages":["Spanish","English"],
        "projects":["prometheus","kubernetes","envoy"],
        "category":["Ambassadors"],
        "email": "johnny!example.com",
        "slack_id": "U123ABC456",
        "image":"jappleseed.jpg"
    }
```

## Images

Upload your headshot image to the [/images/](https://github.com/cncf/people/tree/main/images) directory with a filename made up of your name.  Images should be at least 500x500px, 72dpi, and should be in JPG format with file size less than 100kB.

## Team Management

Also within this repo is a YAML file used by our [automation tooling](https://github.com/electron/sheriff) to help us manage access to resources for teams. This tooling takes advantage of data in [people.json](https://github.com/cncf/people/blob/main/people.json) such as the `email` and `slack_id` fields. This will allow us to add maintainers to different properties only using their GitHub handle.

- To find your Slack ID for the CNCF slack, please follow this [handy guide](https://moshfeu.medium.com/how-to-find-my-member-id-in-slack-workspace-d4bba942e38c)

- When adding your email, please follow the same format used within [devstats](https://github.com/cncf/devstats):

  ```shell
  email!address.xyz
  ```
