class MyStack:
    def __init__(self):
        self.stack = []
    def pop(self):
        if self.is_empty():
            return None
        else:
            return self.stack.pop()
    def push(self,val):
        return self.stack.append(val)

    def peak(self):
        if self.is_empty():
            return None
        else:
            return self.stack[-1]
    def size(self):
        return len(self.stack)
    def is_empty(self):
        return self.size() == 0
        
class BrowserHistory:
    def _init_ (self, backH, fwdH, current):
        self.__backH = MyStack()
        self.__fwdH = MyStack()
        self.__current = ""

    def open(self, url):
        if __current != "":
            __backH.push(__current)
            __fwdH = MyStack
            __current = url

    def back():
        if __backH is Empty():
            print("no history")
        else:
            fwdH.push(__current)
            __current = __backH.pop()

    def forward():
        if __fwdH is Empty():
            print("no way")
        else:
            backH.push(__current)
            __current = __fwdH.pop()

    def printcurrent(self):
        print self.__current

def main():
    bh = BrowserHistory()
    bh.open("")
    bh.open("")
    bh.open("")
    bh.printcurrent()
    bh.back()
    bh.printcurrent()
    bh.forward()
    bh.printcurrent()
    bh.forward()
    bh.printcurrent()
main()
          
