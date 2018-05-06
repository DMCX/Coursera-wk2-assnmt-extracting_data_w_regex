# Coursera-wk2-assnmt-extracting_data_w_regex
Using Python to access data / extracting data with regex (Wk 2 assnmt)

import re
hand = open('regex_sum_93071.txt')
sum = 0
for line in hand:
    line = line.rstrip()
    x = re.findall('[0-9]+', line)
    if len(x) > 0:
        for item in x:
            sum += int(item)

print(sum)
