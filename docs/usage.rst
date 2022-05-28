=====
Usage
=====

To use python-ufile to upload a file::

    import asyncio
    from python_ufile import Ufile
    ufile = Ufile()
    link = asyncio.run(ufile.upload_file("file_name.mp4"))
    print(link)

To use python-ufile to get a temporary link to download a file (it needs API key)::

    import asyncio
    from python_ufile import Ufile
    ufile = Ufile("API_KEY")
    link = asyncio.run(ufile.download_file_link("SLUG"))
    print(link)

To use python-ufile to download a file (it needs API key)::

    import asyncio
    from python_ufile import Ufile
    ufile = Ufile("API_KEY")
    asyncio.run(ufile.download_file("SLUG", "output.mp4"))

