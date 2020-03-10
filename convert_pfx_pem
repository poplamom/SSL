import os

root_dir = 'C:/Program Files (x86)/GnuWin32/bin/pfx'
the_list = ["list1", "list2"]

for x in the_list:
    print(x)
    os.chdir('Z:/'+x)
    os.system('openssl pkcs12 -in ' + x + '_cert.pfx -out ' + x + 'cert.pem -nodes -password pass:[Password]')
    os.system('dir')
    # print(x)

for directory, subdirectories, files in os.walk(root_dir):
    for file in files:
        print(os.path.join(file))
        print(file.split(".")[0] + ".pem")

os.chdir('C:/Program Files (x86)/GnuWin32/bin/')

