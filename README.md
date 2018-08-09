#写一个遍历 names 列表以创建 usernames 列表的 for 循环。要为每个姓名创建用户名，使姓名全小写并用下划线代替空格。对以下列表运行 for 循环： 
#names = ["Joey Tribbiani", "Monica Geller", "Chandler Bing", "Phoebe Buffay"] 
#应该会创建列表：
#usernames = ["joey_tribbiani", "monica_geller", "chandler_bing", "phoebe_buffay"]
names = ["Joey Tribbiani", "Monica Geller", "Chandler Bing", "Phoebe Buffay"] 
usernames=[]
for name in names:
    usernames.append(name.lower().replace(" ","_'))
print(usernames)

names = ["Joey Tribbiani", "Monica Geller", "Chandler Bing", "Phoebe Buffay"] 
for i in range(len(names))
    names[i]+=names[i].lower().replace(" ","_")
print(names)

#写一个 for 循环，用于遍历字符串列表 tokens 并数一下有多少个 XML 标记。XML 是一种类似于 HTML 的数据语言。如果某个字符串以左尖括号“<”开始并以右尖括号“>”结束，则是 XML 标记。使用 count 记录这种标记的数量。
#你可以假设该字符串列表不包含空字符串。
tokens = ['<greeting>', 'Hello World!', '</greeting>']
count=0
for token in tokens:
    if token[0]=="<" and token[-1]==">":
        count+=1
print(count)

#写一个 for 循环，用于遍历字符串列表并创建单个字符串 html_str，它是一个 HTML 列表。例如，如果列表是 items = ['first string', 'second string]，输出 html_str 应该会输出：
#<ul>
#<li>first string</li>
#<li>second string</li>
#</ul>
#即该字符串的第一行应该是起始标记 <ul>。然后是源列表中的每个元素各占一行，两边是 <li> 和 </li> 标记。该字符串的最后一行应该是结束标记 </ul>。
items = ['first string', 'second string']
html_str="<ul>\n"
for item in items:
    html_str+="<li>{}</li>\n".format(item)
html_str+="</ul>"
print(html_str)

