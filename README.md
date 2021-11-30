# p2.khademzadeh
from multiprocessing import Process
import os
def test():
print("process ID is: " + str( os.getpid() ))
if __name__ == '__main__':
print("main process ID is: " + str( os.getpid() ))
p = Process(target=test)
p.start()
p.join()
