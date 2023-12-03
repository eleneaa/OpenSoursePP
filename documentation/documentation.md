**table of contents**

* [Introduction](#introduction)

	* [About the service](#about-service)

	* [Key features ](#features)

* [Tutorials](#tutorials)

	* [Adding newsfeeds](#adding-newsfeeds)

	* [Configuring integration with OpenAi](#OpenAi)

	* [Creating rules](#creating-rules)

	* [News sorting](#sorting)

* [Tab Description](#tab-description)

	* [News](#news)

	* [Feeds](#feeds)

	* [Rules](#rules)

	* [Discovery](#discover)

	* [Collections](#collections)

	* [Settings](#settings)

* [Description of the service’s operation](#description)

	* [Frequency of news loading](#frequency)

	* [Tagging](#assigning-tags)

* [Additional information](#addition)

	* [Project File and Structure Description](#description-files)

	* [Supported formats of news sources](#supported-forms)

* [FAQ](#faq)



<!-- headings -->




## Introduction



<a id="about-service"></a>

### About the service

Feeds Fun is an advanced tool for those who want to stay up-to-date with the latest news. It is a smart system that automatically analyzes and tags all news using ChatGPT, and you can just enjoy the most interesting ones filtered by your individual rules. We understand that everyone has different interests, so we have provided the ability to add up to 50-100 tags to each individual news item, which allows you to customize your rules as precisely as possible.



<a id="features"></a>

### Key features

Key features of Feeds Fun include:



* Managing news feeds, including configuring automatic tagging of news items.

* Setting up news rating algorithms based on specified tags.

* Applying filters to exclude or show news with specific tags.

* Sorting news content by rating, publication date, and other parameters.

* Tracking the news you have already read.

* Supporting both multi-user and single-user modes.



<image style="max-width: 100%; height: auto;" src="images\introduction.png" alt="introduction">



<a id="tutorials"></a>

## Tutorials



<a id="adding-newsfeeds"></a>

### Adding newsfeeds



1. Find the website that hosts the desired news feed

2. Copy the website link (e.g., https://ria.ru/)

3. Paste the link in the Search for a Feed field in the Discovery section

<image style="max-width: 100%; height: auto;" src="images\addingNewsfeeds1.png" alt="figure 1">

4. There may be two options:

    4.1. If the algorithm reads the necessary website as a source, then the links will appear in the Discovery section on the website https://feeds.fun/discovery

<image style="max-width: 100%; height: auto;" src="images\addingNewsfeeds2.png" alt="figure 2">

	4.2 You need to enter the link (e.g. https://www.e1.ru/) in the field if the algorithm does not read this news source. If this is the case, perform the following action

<image style="max-width: 100%; height: auto;" src="images\addingNewsfeeds3.png" alt="figure 3">

5. If the algorithm is not executed correctly, you need to find a new source until you are satisfied with the requirements of the website and the algorithm reads it.



There is also an option to exchange structured information between applications running on different operating systems, which is called OPML:



1. You need to go to the Discovery section.

2. Find Lood feeds from an OPML file on it.

<p><image style="max-width: 100%; height: auto;" src="images\addingNewsfeeds4.png" alt="figure 4">

3. Click the “add file” button and if the file has a suitable type, the upload will be successful.



<a id="OpenAi"></a>

### Configuring integration with OpenAi



1. Go to https://platform.openai.com and log in to your account.

2. Expand the left-hand navigation menu and go to “API”.

3. We recommend creating a separate key for Feeds Fun.

4. Copy the created key.

5. Go to feeds.fun and click on “Settings”, then click on “Edit” in “OpenAI API key”.

6. Paste the key and click “Save”.

7. Optionally, adjust other settings.

8. Go back to the openai website and open the “Settings” tab, then “Billing”.

9. If you recently created an openai account, you will have a trial bonus. Otherwise, you need to top up your balance to the amount you want so that Feeds Fun can use the key.



That’s all, have a nice experience and thank you for supporting the project!



<a id="creating-rules"></a>

### Creating rules

1. Select an article

	The News tab contains a large number of articles. Select the title you like and click on it.

2. Click on a tag

	When you read an article, you can select one or more tags that most accurately describe its content. Click on the corresponding tag that appears under the article’s title. If you want to see all the tags related to the article, click “more.”

3. Add additional tags (optional)

	If you think that one tag is not enough to accurately describe the news, you can add additional tags. To do this, simply click on several tags at once.

<image style="max-width: 100%; height: auto;" src="images\creatingRules2.png" alt="figure 2">

4. Set the tag rating

	Each tag can be assigned a rating that reflects your interest in this topic. For example, for the “sport” tag, you can set a high rating if you are interested in sports, and for the “mathematics” tag, a low rating if mathematics does not interest you.

<image style="max-width: 100%; height: auto;" src="images\creatingRules1.png" alt="figure 1">

5. Click “create rule”

	After you have selected the tags and set the rating for each of them, click the “create rule” button. The program will save your rule by associating the selected tags with the ratings you assigned to them. The list of news will be updated immediately after you create the rule.

6. Organizing news according to your preferences

	After creating rules, the program will filter and sort news according to your preferences. The rating for each tag will be taken into account when determining the priority of news.

7. Improving rules and algorithm

	After you start using the program for reading news with tags, you may need to make changes and improve its performance. If you find that some rules give unwanted results, you can always edit the rules to optimize the algorithm and get more relevant news for you.



<a id="sorting"></a>

### News sorting

1. Sorting options

	Open the News tab. In the upper left corner, there is a list of filters for sorting

	1.1 Time range selector. In the For field, select the time range value

<image style="max-width: 100%; height: auto;" src="images\newsSorting1.png" alt="Figure 1">

	1.2 Sorting type selection. In the Sort by field, select the sorting type:

<image style="max-width: 100%; height: auto;" src="images\newsSorting2.png" alt="Figure 2">

	– Score - sort by descending tag rating. The tag rating is set when creating rules.

	– Score ~ 0 - sort by tags whose rating is approximately equal to 0

	– Score backward - sort by ascending tag rating. The tag rating is set when creating rules.

	– Published - sort by the newest articles

	– Cataloged - sort by the time of news entry into the service database

	1.3 Tag selection. From the resulting news selection, a list of tags assigned to articles is formed, indicating the number of articles with this tag

<image style="max-width: 100%; height: auto;" src="images\newsSorting3.png" alt="Figure 3">

	– Specific tags can be found by writing the tag completely or its part in the Input part of the tag… field

<p><image style="max-width: 100%; height: auto;" src="images\newsSorting4.png" alt="Figure 4">

2. Display options

	2.1 The Show read option controls whether read news are displayed in the general list

	2.2 The Show tags option controls whether tags are displayed in the news list (Figures 5, 6)

<image style="max-width: 100%; height: auto;" src="images\newsSorting3.png" alt="Figure 5">

<image style="max-width: 100%; height: auto;" src="images\newsSorting3.png" alt="Figure 6">





<a id="tab-description"></a>

## Tab Description



<a id="news"></a>

### News

In the “News” tab, the user can conveniently read and sort articles by various parameters. In this section, the user can find the latest news with the tags they are interested in. Each news item is accompanied by tags, which the user can rate ([tutorial for creating rules](#creating-rules)).

On the left panel, there are filters that allow you to configure the display of news by selected parameters. You can sort news by upload date, the presence of tags, or hide already read news. One of the useful functions is the ability to select tags that must be present in articles or, conversely, tags that should not be present in articles ([tutorial for news sorting](#sorting)).

Initially, all news is displayed in chronological order, but with the help of filters, the user can change the sorting of the news list in accordance with their preferences.



<image style="max-width: 100%; height: auto;" src="images\news.png" alt="Figure 6">



<a id="feeds"></a>

### Feeds



1. This tab has filtering options for added news:

	- title sorting by headings

	- URL sorting by URLs

	- loaded sorting by loading times

	- added sorting by addition times

Show descriptions - is responsible for displaying link descriptions

Show failed - is responsible for the order of displaying links with errors You can also refresh the list of news.

2. To view the page content, you can click on the link.

3. There is a deletion of news that is available on the site, as well as the date of its publication and the time of its modification.



<image style="max-width: 100%; height: auto;" src="images\feeds.png" alt="Figure 6">



<a id="rules"></a>

### Rules

In this tab, you can view all rules created by you (detailed tutorial for creating rules: [Creating rules](#creating-rules)).

<image style="max-width: 100%; height: auto;" src="images\rules1.png" alt="Figure 1">

Also:



1. Change the rating of an already created rule or delete the rule itself

<image style="max-width: 100%; height: auto;" src="images\rules2.png" alt="Figure 2">

2. Sort rules by tags, rating, date of creation, and date of update

<image style="max-width: 100%; height: auto;" src="images\rules3.png" alt="Figure 3">

3. From the resulting selection of rules, a list of tags selected in the rules is formed, indicating the number of rules with this tag (pic.5)



– Certain tags can be found by writing the tag completely or partially in the Input part of the tag… field (pic.6)



<a id="discover"></a>

### Discovery

In the Discovery tab, you can add new sources of articles, there is also an option to exchange structured information between applications running on OPML. Detailed tutorial: [Adding news sources](#adding-newsfeeds)



<image style="max-width: 100%; height: auto;" src="images\discovery.png" alt="Figure 6">





<a id="collections"></a>

### Collections

This section allows you to add your own news feeds using OpenAI tokens. By default, we have 2 news feed sections:



1. Gamedev

2. Artificial Intelligence



Also you can also subscribe for tokens.



<p><image style="max-width: 100%; height: auto;" src="images\Collections1.png" alt="Figure 6">



<a id="settings"></a>

### Settings



1. There is a user id in the section.

<p><image style="max-width: 100%; height: auto;" src="images\settings1.png" alt="Figure 1">

2. You can set access to Open AI.

<image style="max-width: 100%; height: auto;" src="images\settings2.png" alt="Figure 2">

3. How many tokens can be in the site, in your account

<image style="max-width: 100%; height: auto;" src="images\settings3.png" alt="Figure 3">

4. When using the Open AI key, there’s a rule for the users so that the users don’t spend a lot of tokens. You can set news by date added, for example not older than 3 days.

<image style="max-width: 100%; height: auto;" src="images\settings4.png" alt="Figure 4">

5. You can see the number of used tokens in processed requests, reserved tokens for requests, and how many total tokens were used in a month.

<image style="max-width: 100%; height: auto;" src="images\settings5.png" alt="Figure 5">



<a id="description"></a>

## Description of the service’s operation



<a id="frequency"></a>

### Frequency of news loading



<a id="assigning-tags"></a>

### Tagging

In the Feeds Fun system, ChatGPT plays a key role in the formation of tags. Using artificial intelligence, the system analyzes the content of the article and automatically assigns relevant tags.

The processes for determining tags are performed using processors located in the librarian/processors directory.



<image style="max-width: 100%; height: auto;" src="images\tegging1.png" alt="Figure 1">



The main code for working with OpenAI is located in the librarian/processors/openai_chat_3_5.py file. We send a request that includes the text of the article, and we get relevant tags in response.



<image style="max-width: 100%; height: auto;" src="images\tegging2.png" alt="Figure 2">



Feeds Fun also complements its list of tags from the following sources:



-Meta tags of the site: Information from the meta tags of the site from which the article was taken is used to determine tags.

-Content of the news: If the source provides tags within the news itself, Feeds Fun also takes them into account when forming the list of tags.

-Site title: Based on the site title, a special tag named “upper-case-title” is created.



Native tags are obtained using the feedparser module.



<image style="max-width: 100%; height: auto;" src="images\tegging3.png" alt="Figure 3">



Tagging the “upper-case-title” tag in the code occurs in this way:



<image style="max-width: 100%; height: auto;" src="images\tegging4.png" alt="Figure 4">



This integrated approach allows the system to take into account various sources of information, ensuring accuracy and diversity in the formation of tags for each article.



<a id="addition"></a>

## Additional information



<a id="description-files"></a>

### Project File and Structure Description

```

ffun:

	api:

		enities.py  - definition of basic program classes such as Feed, Entry, UserSetting

		http_handlers - HTTP request handlers for a web application



	>!application:

		application.py - contains the main code for creating and configuring FastAPI-based Web application through it

	>!settings.py - contains settings for PostgreSQL, settings of the application itself: name, domain, port, etc.

	user_settins.py - description of user openai settings.

	>!workers.py - functions to start background processes, loader and feed library



	auth:

		directory with authorization code in bot via mail



	cli:

		command line functionality

	core:

		 fundamental logic, basic utilities and general functions



	domain:

		urls.py - file to normalize links



	feeds:

		entities.py - FeedError:

				network_unknown = 1000

				network_no_address_associated_with_hostname = 1001

				network_name_or_service_not_known = 1002

				network_certificate_verify_failed = 1003

				network_connection_timeout = 1004

				network_read_timeout = 1005

				network_illegal_request_line = 1006

				network_non_200_status_code = 1007

				network_disconection_without_response = 1008

				network_undetected_connection_error = 1009

				network_unsupported_protocol = 1010

				network_server_breaks_connection = 1011

				network_could_not_resolve_host = 1012



				parsing_unknown = 2000

				parsing_base_error = 2001

				parsing_format_error = 2002

				parsing_unicode_decode_error = 2003

				parsing_feed_content_not_found = 2004



				protocol_unknown = 3000

				protocol_no_entries_in_feed = 3001



			FeedState:

				not_loaded = 1

				loaded = 2

				damaged = 3

				orphaned = 4



		operations.py - operations with database of feeds



	>!feeds_collections:

		>!collections:

			directory with api links to sites with articles for parsing, for example "http://www.reddit.com/r/proceduralgeneration/.rss", in general directory to work with collections from links to resources with articles



	feeds_discoverer:

		domain.py - provides functions for working with domains and extracting tape information (feed) from websites



	feeds_link:

		directory to manage the database of links to sites with articles, functions of adding the user, removal function etc.



	librarian:

		functionality for article processing, tagging



	library:

		work with database of articles, addition to database, tests with database output



	>!loader - one of the main folders:

 uses many functions of the project:  content downloading, content decoding, content parsing, downloading content using proxy on server and etc

		>!settings.py - loader settings: number of loaders, minimum period between data downloads, proxy.



	markers:

		work with database, mark about the article read and delete mark.



	ontology:

		work with tags, add deletion to database



	openai:

		all work with a neural network, queries for it, getting answers, calculating the number of used



	parsers:

		code for parser article for example from "http://www.reddit.com/r/proceduralgeneration/.rss"



	resources:

		domain.py - contains the month start function

		In the main contains work with the user base



	scores:

		work with tag priorities



	tags:

		normalization tags



	user_settings:

		work with us_settings database table



	users:

		 create user_id and add to the table u_mapping

```





<a id="supported-forms"></a>

### Supported formats of news sources



<a id="faq"></a>

## FAQ

