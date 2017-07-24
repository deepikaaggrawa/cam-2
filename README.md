
lines = []

with open('sources.txt', 'rt') as in_file:

    for line in in_file:
    
        lines.append(line.rstrip('\n'))
for element in lines:
    if not "http" in element:
        data = element.split(':')[0]
        print(data)
