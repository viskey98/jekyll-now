---
layout: post
title: GSoC week-2
---
This is the second week of `GSoc 2018`

# Report
I have started reconstructing [SNARE](http://github.com/mushorg/snare).

* Step 1:

  I have broken current snare into 2 files :
  * snare.py:
    * Contains every functions in snare except HttpRequestHandler class. 
  * server.py:
    * Contains the HttpRequestHandler class.
* Step 2:

  Server was further broken down into 3 files:
  * server.py
    * `handle_request()`
  * html_handler.py
    * `get_dorks()`
    * `handle_content()`
      * Function handle_html_content from server.py renamed to handle_conent
  * tanner_hanlder.py
    * `submit_slurp()`
    * `create_data()`
    * `submit_data()`
    * `parse_tanner_response()`
* Step 3:

  Snare was further broken down into 4 files:
    * snare.py
      * `main()`function of snare
    * startup.py
      * `create_initial_config()`
      * `snare_setup()`
      * `drop_priviliges()`
      * `compare_version_info()`
      * `check_tanner()`
    * utils/tag_adder.py
      * `add_meta_tag()`
      * `parse_timeout()`
