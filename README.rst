.. include:: cyverse_rst_defined_substitutions.txt
.. include:: links.rst

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

CyVerse Austria  Workshop
-------------------------

**Location**: Technical University of Graz Lehrsaal VI (FS EG 076)
Inffeldgasse 11 (with TUG Wifi)


This "Train-the-trainer" style workshop will be a week-long collaboration
between CyVerse trainers and staff from CyVerse US as well as trainers and staff
from CyVerse Austria. Over the week, the goal will be to help each CyVerse
Austria trainer:

1. Know the basic capabilities of CyVerse Austria infrastructure
2. Give feedback to shape the development of CyVerse Austria infrastructure
3. Be able to customize and install tools required by CyVerse Austria users
4. Develop effective training and documentation skills to make CyVerse Austria
   a success for its users.

Currently, the CyVerse Austria cyberinfrastructure implements key capabilities
of CyVerse infrastructure:

- **Data Store:** Data storage, sharing, metadata management,
- **Discovery Environment:** A web-based, graphical interface to hundreds of
  bioinformatics tools
- **Visual and Interactive Computing Environment**: Jupyter labs, RStudio, and
  RShiny applications easily launched and managed in the Discovery Environment

-----

Pre-Workshop Setup
---------------------

**Minimum Setup Instructions**

We ask that all attendees download/install the following software tools prior
to the workshop. If you have any difficulty, we will have time to help you with
installation problems during the workshop.

**Hardware/Software**

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Notes
      - Links
    * - Wi-Fi-enabled laptop (Mac or Linux recommended)
      - You should be able to use CyVerse from any laptop using
        Windows/MacOS/Linux. We **Strongly recommend** having access to a laptop
        running Windows/MacOS. While you will be able to use CyVerse components
        from any laptop, some of the tool installations may work better with
        those operating systems. If you are using Windows, you may wish to
        install |Linux Bash for Windows|.
        We also **strongly recommend** Firefox or Chrome browser; **We do not**
        **recommend Microsoft Edge Browser**. It is helpful if you have
        administrative/install permissions on your laptop. **Note:** If
        specified, some workshops will be held in computer labs in which case a
        laptop is optional.
      - - |Download FireFox|
        - |Download Chrome|
    * - Cyberduck
      - Cyberduck is a third-party tool for uploading/downloading data to CyVerse.
        Currently, this tool is available for Windows/MacOS only. You will need
        to download Cyberduck and the connection profile. We will go through
        configuration and installation at the workshop.
      - |Download Cyberduck|
    * - Docker
      - Docker is a technology for running individual software tools in a
        reproducible environment, and on any machine. We request you install
        The **Desktop, Community Edition** of Docker if you are using
        Windows or MacOS. The **Docker CE x86_64** instructions are also
        available for Linux users. If you have installation problems, we
        will also have backup cloud instances available.
      - |Download Docker|
    * - Git
      - Git is a version control software.
        If you are using Linux or MacOS, you most likely already have Git.
        Windows users may need to install Git. You can find instructions
        for Git installation at the link.
      - |Install Git|
    * - Text editor
      - You will need to have a text editor suitable for working with code
        (*Not* Microsoft word, or other word processing software).
      - We recommend installing |Atom|
    * - Python (optional)
      - For our documentation you will need Python 3 (3.8.0 or later) installed.
        this is likely already installed on Linux/MacOS systems
      - |Install Python|
    * - Python package manager PIP (optional)
      - For our documentation you will need Python 3 (3.8.0 or later) installed
      - |Install Python PIP|
    * - Python sphinx (optional)
      - For our documentation you will need sphinx and themes
      -  .. code-block:: bash

            # run this command at the terminal

            $ pip install sphinx
            $ pip install sphinx-autobuild
            $ pip install sphinx_rtd_theme
    * - Python RestView (optional)
      - For our documentation |RestView|
        documentation.
      -  .. code-block:: bash

             # run this command at the terminal

             $ pip install restview


**Accounts**

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Notes
      - Links
    * - CyVerse Austria Account
      - Please ensure you have a CyVerse account and have **verified** your
        account by completing the verification steps in the email you got when
        you registered. You can **test your account** by logging
        into |CyVerse Austria User Portal|.
      - Register for your CyVerse account at |CyVerse Austria User Portal|.
        Please register using an institutional email address (e.g.
        .edu/.gov/.org etc.).
    * - Github
      - We will make use of Github for managing documentation, and also any
        software/scripts developed (E.g. Docker files).
      - Register for a |GitHub| account
    * - Dockerhub
      - Dockerhub is an online repository for the sharing and management of
        Docker images.
      - Register for a |Dockerhub| account
    * - University VPN
      - If you want to access data located at your home institution, you may
        want to have VPN (virtual private network) software installed.
      - Contact your university IT department if you need assistance.

**Optional and Extras**

These are some extra steps that aren't required for the workshop, but which
provide some options for functionalities we will cover.

.. list-table::
    :header-rows: 1

    * - Tool
      - Notes
      - Link
    * - VNC Viewer
      - This tool enables connection to a remote Atmosphere Desktop. No installation
        or configuration is needed.
      - |Download VNC Viewer|
    * - PuTTY (windows only)
      - PuTTY allows SSH connection to a remote machine, and is designed for
        Windows users who do not have a Mac/Linux terminal.
      - |Download PuTTY|
    * - iCommands
      - iCommands are third-party software for command-line connection to the
        CyVerse Data Store.
      - Download and installation instructions available at |CyVerse Learning Center - iCommands|

-----

Slack
````````

We will Slack for shared notes and easy exchange of
code, feedback, links, etc.: **TBA**

-----

Important links
--------------------

- CyVerse Austria User Portal: `https://user.cyverse.tugraz.at/ <https://user.cyverse.tugraz.at/>`_
- CyVerse Austria Discovery Environment: `https://de.cyverse.tugraz.at/ <https://de.cyverse.tugraz.at/>`_
- CyVerse Austria Data Store configuration:
    - irods host: `data.cyverse.tugraz.at`
    - irods zone: `TUG`
    - irods port: `1247`

- Instant Session Feedback: `Feedback form <https://forms.gle/nXibnHhH8wqZzq2s6>`_

----

Agenda
------

This workshop is will be interactive and collaborative (part training workshop,
part coda-a-thon/hack-a-thon). For the most part, mornings will start with
some lectures, discussion, and hands-on exercises. We will then decide as a
group what the afternoon agenda should focus on. We also anticipate that
attendees may want to different things and we will have some capacity to
divide into smaller groups. Everything on the agenda is up for discussion, if
something you would like to see is missing we can add it!

Monday 2019-11-18
`````````````````

**Learning activities and goals**

- Answer questions about how CyVerse can be used
- Explore what is possible now, possible soon, and what needs to be made
  possible
- Get a basic understanding of how to use CyVerse to handle common
  data management tasks (Data import, sharing, and publication)


.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 09:00-09:30
      - Computational Thinking with CyVerse
      -
      -
      -
    * - 09:30-10:00
      - Introductions and user needs discussions
      -
      -
      -
    * - 10:00-10:30
      - Cyberinfrastructure platform overview
      - |DE Slides|
      -
      - |Introduction to CyVerse|
    * - 10:30-11:00
      - **Break**
      -
      -
      -
    * - 11:00-11:30
      - Data Store Basics - Upload/Import
      - |DS Slides|
      - |Data Store Guide|
      - - |Data Management Overview|
        - |Download Cyberduck Austria Profile|
    * - 11:30-12:00
      - Data Store Basics - Metadata templates
      -
      -
      - |Associating Metadata|
    * - 12:30-01:30
      - **Lunch**
      -
      -
      -
    * - 01:30-05:00
      - - **Flexible PM Session** (Break included)
        - Data Store Basics - Data Sharing
        - Data Store Basics - Data Commons
        - Data Store Basics - Data Management Planning
        - Data Store Additional topics - iCommands
      -
      -
      - - |Data Stewardship Wizard|
        - |Plan S principles|

Tuesday 2019-11-19
``````````````````

**Learning activities and goals**

- Get more details on how scientific tools can be deployed on CyVerse
- Learn the value of using Docker containers to manage tool
- Understand how to obtain, deploy, and customize containers
- Make science reproducible with documentation and notebooks


.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 09:00-09:30
      - Data analysis with the Discovery Environment
      -
      -
      - |Discovery Environment Guide|
    * - 09:30-10:00
      - Docker Basics
      -
      -
      - |Introduction to Docker|
    * - 10:00-10:30
      - Docker basics (cont'd)
      -
      -
      -
    * - 10:30-11:00
      - **Break**
      -
      -
      -
    * - 11:00-11:30
      - Docker basics (cont'd)
      -
      -
      -
    * - 11:30-12:00
      - Introduction to  VICE
      -
      -
      - - |Introduction to VICE|
        - |VICE documentation|
    * - 12:30-01:30
      - **Lunch**
      -
      -
      -
    * - 01:30-05:00
      - - **PM Session planning** (Break included)
        - Creating open documentation with ReadTheDocs
        - More on Docker
        - Identifying tools with Bioconda, Biocontainers, Dockerhub
        - More on building Juypyter Notebooks
      -
      -
      - - |CyVerse Documentation Quickstart|
        - |CyVerse Documentation Github|
        - |ReadTheDocs Documentation|
        - |Jupyter Notebook Tutorial|
        - |What is a container|?
        - |Intro Docker tutorial|
        - |Docker docs|

Wednesday 2019-11-20
````````````````````

**Learning activities and goals**

- Work collaboratively on installing tools on CyVerse (DE/VICE)
- Go through the major steps of tool deployment from importing,
  deployment, testing, and documenting.
- Work on and reinforce topics from day I and II


.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 09:00-09:30
      - Tool installation in the Discovery Environment
      -
      -
      - |DE Tool Integration|
    * - 09:30-10:00
      - Tool installation in the Discovery Environment
      -
      -
      -
    * - 10:00-10:30
      - Tool installation in the Discovery Environment
      -
      -
      -
    * - 10:30-11:00
      - **Break**
      -
      -
      -
    * - 11:00-11:30
      - Tool installation in the Discovery Environment
      -
      -
      -
    * - 11:30-12:00
      - Tool installation in the Discovery Environment
      -
      -
      -
    * - 12:30-01:30
      - **Lunch**
      -
      -
      -
    * - 01:30-05:00
      -  - **PM Session planning** (Break included)
         - Building scientific workflows
         - Introduction to Git and Github
         - Planning for day IV, V projects
      -
      -
      - - |Version Control (FOSS)|

Thursday 2019-11-21
```````````````````

**Learning activities and goals**

- Working on complex scientific software (exploring the QIIME use case)
- Individual project development and work


.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 09:00-09:30
      - Introduction to QIIME
      -
      -
      - - |QIIME2 Website|
        - |DNA Subway|
        - |DNA Subway Guide|
        - |DNA Barcoding 101|
    * - 09:30-12:30
      - Individual project work
      -
      -
      - - |Draw.io|
        - |Google Drive for Presentations|
    * - 12:30-01:30
      - **Lunch**
      -
      -
      -
    * - 01:30-05:00
      -  **Report out and PM project work** (Break included)
      -
      -
      -

Friday 2019-11-22
`````````````````

**Learning activities and goals**

- Working on complex scientific software (exploring the QIIME use case)
- Building teaching/training skills
- Review of tools for collaboration
- Group presentations and plans for the future

.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 09:00-09:30
      - Improving your teaching/training skills with Carpentries
      -
      -
      - - |Carpentries Homepage|
        - `Carpentries slide deck <https://de.cyverse.org/dl/d/0D932DF0-4FD5-49BD-B332-2EB4FC72A373/carpentries.pdf>`_
    * - 09:30-10:00
      - Building a local community of practice
      -
      -
      - |LifeSciTrainers Homepage|
    * - 10:00-12:30
      - **Individual Project Work** (Break included)
      -
      -
      -
    * - 12:30-01:30
      - **Lunch**
      -
      -
      -
    * - 01:30-03:00
      - - **Group presentations**
        - Wrap up discussion
        - Individual meetings
      -
      -
      - |Workshop Survey|

-----

Resources Bin
`````````````

These are links to exercises, tutorials, and other learning materials. We may
or may not cover all of these items in the workshop.

.. list-table::
    :header-rows: 1

    * - Resource
      - Description
      - Link
    * - Kallisto RNA-Seq Tutorial
      - RNA-Seq analysis using Kallisto and Sleuth. (Uses DE and RStudio)
      - - |Kalisto tutorial|
        - |Sleuth tutorial|
    * - QIIME2 v2019.10 Jupyter Lab
      - |QIIME2 Jupyter Lab tutorial|
      - |QIIME2|
    * - CyVerse FAQ
      - General CyVerse FAQs
      - |CyVerse FAQ|


-----

Code of Conduct
----------------

This workshop is run under a |Code of Conduct| - please
respect it and your fellow attendees!

-----


About CyVerse
-------------

**CyVerse Vision:** Transforming science through data-driven discovery.

**CyVerse Mission:** Design, deploy, and expand a national
cyberinfrastructure for life sciences research and train scientists in
its use. CyVerse provides life scientists with powerful computational
infrastructure to handle huge datasets and complex analyses, thus
enabling data-driven discovery. Our powerful extensible platforms
provide data storage, bioinformatics tools, image analyses, cloud
services, APIs, and more.

While originally created with the name iPlant Collaborative to serve
U.S. plant science communities, CyVerse cyberinfrastructure is germane
to all life sciences disciplines and works equally well on data from
plants, animals, or microbes. By democratizing access to supercomputing
capabilities, we provide a crucial resource to enable scientists to find
solutions for the future. CyVerse is of, by, and for the community, and
community-driven needs shape our mission. We rely on your feedback to provide
the infrastructure you need most to advance your science, development, and
educational agenda.

**CyVerse Homepage:** `http://www.cyverse.org <http://www.cyverse.org>`_

Funding and Citations
---------------------

CyVerse is funded entirely by the National Science Foundation under
Award Numbers DBI-0735191, DBI-1265383, and DBI-1743442.

Please cite CyVerse appropriately when you make use of our resources,
`CyVerse citation
policy <http://www.cyverse.org/acknowledge-cite-cyverse>`__


.. |Code of Conduct| raw:: html

   <a href="./getting_started/code_of_conduct.html" target="blank">Code of Conduct</a>

.. |QIIME2| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _QIIME2: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=0fe69a8f-216d-4103-abd8-a2080af82876&app-id=58150fe4-01cf-11ea-8c41-008cfa5ae621
