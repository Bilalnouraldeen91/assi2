 def count_digits(n): 
    return 1 if n < 10 else 1 + count_digits(n // 10)

def find_max(lst): 
    return max(lst) if lst else 0

def count_tags(html, tag): 
    open_tag = f"<{tag}>"
    close_tag = f"</{tag}>"
    count = 0
    index = 0

    while index < len(html):
        if html.startswith(open_tag, index):
            count += 1
            index += len(open_tag)
        elif html.startswith(close_tag, index):
            index += len(close_tag)
        else:
            index += 1

    return count

def main(): 
    while True: 
        print("\nMenu:") 
        print("1. Count Digits") 
        print("2. Find Max") 
        print("3. Count Tags") 
        print("4. Exit") 

        choice = input("Enter a choice: ")
       


#####################################################
Hi Johnny! I am a journalist, and honestly, due to the dramatic events taking place right now in Lebanon, 
my job requires me to be on the ground. 
Because of this, I’m unable to focus fully on the assignment, but I’ve made the most of the time I have allowed.
#####################################################
