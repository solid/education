This file contains notes for a beginner Introduction to Solid Workshop. 
This should be accompanied with a Slide Deck for the presentation.

# About Solid

## About the Solid Project

- Decentralized web
- Project started by Sir Tim Berners-Lee; inventor of the World Wide
    Web
- *Solid is an open standard for structuring data, digital identities,
    and applications on the Web.*
- Goal: for people to have more agency over their data
    - **True data ownership** - Users should have the freedom to
        choose where their data resides and who is allowed to access it.
    - **Fully interoperable standards** - Solid uses a common, shared
        way of describing things and their relationships to one another
        that different applications can understand.
        - This gives Solid the unique ability to allow different
            applications to work with the same data.
        - Prevents application vendor lock-in
    - **Granular access --** Solid's authentication and authorization
        mechanisms allow one to determine which people and applications
        can access their data

## Solid in a nutshell

- **Solid is a specification** consisting of several Technical
    Reports, including the Solid Protocol:
    <https://solidproject.org/TR/protocol>
    - *The specifications in the ecosystem describe how Solid servers
        and clients can be interoperable by using Web communication
        protocols, global identifiers, authentication and authorization
        mechanisms, data formats and shapes, and query interfaces.*

- **Solid Pod: Pods are where you store your data**.
    - Any kind of data can be stored in a Solid Pod
        - Structured data, files
    - Linked Data which allows different applications to work with the
        same data
        - *Linked Data is a set of design principles for sharing
            machine-readable interlinked data on the Web.*
    - Once data is in your Pod, you control access to it.

- **Pod Provider:**
    - You can get a Pod from a Pod Provider, or you can self-host your
        Pod. (You can also implement a new Pod Provider if you like
        implementing from specifications!)
    - <https://solidproject.org/users/get-a-pod>
        - Many Pod Providers to choose from! Some community-based,
            some by companies.
        - A Pod Provider will usually advertise the underlying cloud
            infrastructure it is using, and the hosting location. For
            example, Inrupt Pod Spaces uses Amazon for hosting and the
            hosting location is Germany.

- **Solid applications:**
    - Any type of application can be built using the Solid Protocol.
    - Applications can make requests to retrieve data from your Pod (via your Pod Provider), and also to store data on your Pod. This is the essential part of how Solid works. 
        - Keep in mind that you ALWAYS control access of your files on your Pod, so you can revoke access to an application at any time. 
    - Catalog of applications, people, organizations, and other things in Solid:
        - <https://solid-catalog.jeswr.org> or <https://solidproject.solidcommunity.net/catalog/>
        - <https://solidproject.org/apps> 
    - Example actively funded projects:
        - health care use case (name?) by Marc Haddle
        - ???

## Solid in context

- Solid is a specification consisting of several Technical Reports,
    each edited by a Solid panel.
    - Anyone can contribute by [filing an issue on
        GitHub](https://github.com/solid/specification/issues)
    - Technical Reports: <https://solidproject.org/TR/> include the
        [Solid Protocol](https://solidproject.org/TR/protocol), [Solid
        WebID Profile](https://solid.github.io/webid-profile/), [Web
        Access Control](https://solidproject.org/TR/wac), [Shape
        Trees](https://shapetrees.org/TR/specification/), [Solid
        Chat](https://solid.github.io/chat/), and lots more!

- The authors of the technical reports are the [Solid Community
    Group](https://www.w3.org/groups/cg/solid/) (CG) and the Linked Web Storage Working Group (LWS WG) of the
    [W3C](https://www.w3.org/).
    - W3C is the World Wide Web Consortium: they *develop standards
        and guidelines to help everyone build a web based on the
        principles of accessibility, internationalization, privacy and
        security.*. They endorse the Solid Project officially through the LWS Working Group.

- Solid has a new organizational home, the Open Data Institute (ODI),
    as announced by Sir Tim Berners-Lee on October 2024. [Link to
    post](https://forum.solidproject.org/t/a-new-organisational-home-for-solid/8004)
    - The ODI is a non-profit institute that aims to build a world where
        data works for everyone. It was founded in 2012 by Sir Tim
        Berners-Lee and Sir Nigel Shadbolt.

- Solid community channels
    - Solid Forum: <https://forum.solidproject.org/>
    - Matrix channels:
        [https://matrix.to/#/#solid_project:matrix.org](https://matrix.to/#/#solid_project:matrix.org)
    - Solid Practitioners Bi-Weekly meeting:
        - https://www.w3.org/events/meetings/ba3d6036-ef79-42f1-acc7-8ce9d3bc00ba/20271007T150000/
        - <https://www.w3.org/events/meetings/b2bcc109-a7e7-4e9c-ba9f-8dcd234e5275/20270916T150000/>
    - Community Group (CG) meeting [https://www.w3.org/community/solid/](https://www.w3.org/community/solid/)
    - SolidOS meetings [https://github.com/SolidOS/solidos](https://github.com/SolidOS/solidos) for those with some experience with Solid that want to contribute to SolidOS
    - Active community of Solid enthusiasts, developers from companies
        and non-profits!

## Why do we need Solid? 

- Solid empowers end-users (you and I) to reclaim ownership of our own
    data on the Web. Currently all our personal data is stored on
    companies' servers, where they have custody of the data. Solid
    provides a technical solution to end-users having their own agency
    to their data, how it is used and who it is used by.
- Privacy and Data Ownership
    - Individuals and organizations can have their own Pods to store
        their data.
    - They have control over access; which individuals or applications
        access their data, and they can revoke this access at any poin
- Application Interoperability
    - You can use multiple applications at the same time, with the
        same data, without duplication of data.
- Untangle Network Effects
    - Applications no longer need to take care of managing servers to
        host user data. They can focus on their application itself.
- List of domain areas that can benefit from Solid (written by Sir Tim
    Berners-Lee in
    [*DesignIssues/Vision*](https://www.w3.org/DesignIssues/Vision.html))

    - calendars, to-dos, app stores, contacts, blogs, podcast, chat,
        conference management, education, tuition, employment, taxes,
        finances, banking; fitness, gaming, benefits, government
        services, healthcare, legal, media creation and mixing,
        professional profiles, recipes, nutrition, refugee handling,
        retail, and, travel.

# Hands-on Activity

The workshop activity ideally should involve creating a basic Solid application (eg. React to-do list app) using an existing Pod Provider.

Ideas on workshop activity (todo: add more / a new workshop activity guide):

- https://solidproject.org/developers/tutorials/getting-started
        - O.Team offers the [Solid-React-LDO tutorial](https://ldo.js.org/guides/solid_react/).
	- Inrupt offers <https://docs.inrupt.com/developer-tools/javascript/client-libraries/tutorial/getting-started>
- a guide: https://rdfjs.dev/solid 

# Follow-up workshop ideas

- How to self-host a Pod Provider
- A short workshop series on how to implement your own (simple) Pod Provider
- Additional workshops on creating Solid apps while learning more about the technologies, specs and theory
 
# References

- <https://www.ateam-oracle.com/post/an-introduction-to-solid>
- <https://solidproject.org/about>
- <https://solidproject.org/specification>
- <https://theodi.org/about-the-odi/our-vision/>
- <https://noeldemartin.com/blog/why-solid>
- <https://solidproject.org/TR/protocol>
- <https://www.ontotext.com/knowledgehub/fundamentals/linked-data-linked-open-data/>
- <https://solidproject.org/users/get-a-pod>
- <https://solidproject.org/apps>
- <https://www.w3.org/DesignIssues/Vision.html>
