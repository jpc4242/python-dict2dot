# python-dict2dot

Python Dictionary to **Dot notation** published in
[GitHub](https://github.com/nandoabreu/python-dict2dot) and 
[PyPi](https://pypi.org/project/python-dict2dot/).  

This implementation admits dot notation to access nested dictionaries, once the parent is dict.

To pip install, run:  

    $ pip install dict2dot

&nbsp;  
&nbsp;  
## The main class
With the python console and the [dict2doc package](dict2dot/__init__.py), we can get things running:

    $ python

    >>>
    from dict2dot import Dict2Dot

    my_d2dot = Dict2Dot({'dogs': {'breeds': ['Golden']}, 'birds': {'breeds': ['Cockatiel']}})
    my_d2dot.dogs.breeds.append('Lhasa Apso')
    print( my_d2dot.dogs )

    my_dict = my_d2dot.dict()
    print( my_dict )

    other_dot2dict = Dict2Dot()
    other_dot2dict.a_new_key = 'a new value'
    print( other_dot2dict.a_new_key )


## Documentation
Please try from python console:

    $ python
    >>> from dict2dot import Dict2Dot
    >>> help(Dict2Dot)

Or try from command line:

    $ python -c "import dict2dot; print(dict2dot.__doc__)"

All documentation can be found in [docs](docs).


## To do

* Remove elements from class.
* Improve documentation.

