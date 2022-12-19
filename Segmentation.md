from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Toilets"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Bathroom sinks"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
---------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Showerheads"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
----------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Bathroom Tile"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
---------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Vanities"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Faucets"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Lighting"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
---------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Cabinets & Storage"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Bathtubs and Whirlpools"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-----------------------------------------------------------------------------------
from serpapi import GoogleSearch
import os, json

image_results = []

for query in ["Showers"]:
    params = {
        "engine": "google",               # search engine. Google, Bing, Yahoo, Naver, Baidu...
        "q": query,                       # search query
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("af38279922138da02b23f7864f1264a45f5ae85383fc09760e62dc8f73855217")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
----------------------------------------------------------------------------------
