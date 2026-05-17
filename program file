book_collection = {
    "to_read": set("Atomic Habits,Confession,HTML".split(",")),
    "read": set("Rich dad Poor dad,Go pro,python for beginners".split(","))
}

def add_book(title):
    if title in book_collection["to_read"] or title in book_collection["read"]:
        print(f"'{title}' is already in your list.")
    else:
        book_collection["to_read"].add(title)
        print(f"'{title}' added to your reading list.")

def edit_book(old_title, new_title):
    if old_title in book_collection["to_read"]:
        book_collection["to_read"].remove(old_title)
        book_collection["to_read"].add(new_title)
        print(f"Updated '{old_title}' to '{new_title}' in 'to_read' list.")
    elif old_title in book_collection["read"]:
        book_collection["read"].remove(old_title)
        book_collection["read"].add(new_title)
        print(f"Updated '{old_title}' to '{new_title}' in 'read' list.")
    else:
        print(f"'{old_title}' not found in your collection.")
def remove_book(title):
    if title in book_collection["to_read"]:
        book_collection["to_read"].remove(title)
        print(f"'{title}' removed from 'to_read' list.")
    elif title in book_collection["read"]:
        book_collection["read"].remove(title)
        print(f"'{title}' removed from 'read' list.")
    else:
        print(f"'{title}' not found in any list.")

def mark_as_read(title):
    if title in book_collection["to_read"]:
        book_collection["to_read"].remove(title)
        book_collection["read"].add(title)
        print(f"'{title}' removed from 'read' list.")
    else:
        print(f"'{title}' not found in any list.")

def mark_as_read(title):
    if title in book_collection["to_read"]:
        book_collection["to_read"].remove(title)
        book_collection["read"].add(title)
        print(f"Marked '{title}' as read.")
    else:
        print(f"'{title}' is not in your to-read list.")

def show_books():
    print("\n📘 Books to Read:")
    for b in book_collection["to_read"]:
        print(" -", b)
        print("\n✅ Books Read:")
        for b in book_collection["read"]:
          print(" -", b)
    
def low_stock_alert():
    if len(book_collection["to_read"]) < 2:
        print("⚠️  Low stock alert: You have less than 2 books left to read!")

def search_book(title):
    if title in book_collection["to_read"]:
        print(f"'{title}' is in your to-read list.")
    elif title in book_collection["read"]:
        print(f"'{title}' is in your read list.")
    else:
        print(f"'{title}' not found in your collection.")

def usage_summary():
    print("\n📊 Summary:")
    print(f"Books to Read: {len(book_collection['to_read'])}")
    print(f"Books Read: {len(book_collection['read'])}")
    print(f"Total Books: {len(book_collection['to_read']) + len(book_collection['read'])}")


# Example Usage 
add_book("The 48 Laws of Power")
mark_as_read("HTML")
edit_book("Confession", "Crime and Punishment")
remove_book("Go pro")
search_book("Atomic Habits")
show_books()
usage_summary()
low_stock_alert()
