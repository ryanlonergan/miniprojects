I started this project as I wanted to write some code to find the days remaining between two dates. After doing so and realizing how simple it was, I noticed I had never fully explored the datetime package despite using it extensively for work. To help familiarize myself more with it, I found a set of exercises from w3 schools and am currently working my way through them. The exercises can be found <a href="https://www.w3resource.com/python-exercises/date-time-exercise/"> here</a> and the code I originally set out to write is:

    import datetime

    start_date = datetime.date.today()
    end_date =  datetime.date(YEAR, MONTH, DAY)

    time_delta = end_date - start_date

    print(time_delta.days)