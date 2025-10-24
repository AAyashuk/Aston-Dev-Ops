#!/bin/bash
read URL
if curl "$URL" > /dev/null; 
then
echo "Resource $URL is available"
exit 0
else
echo "Resource $URL is not available"
exit 1
fi