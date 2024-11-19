# container_of
**How to use container_of function of linux kernel?**

```
struct container {
  int some_other_data;
  int this_data;
}

thi_data_ptr // This is a pointer pointing to this_data.

struct container *my_container = container_of(thi_data_ptr, struct container, this_data);

```

You do not know the address of the start of the structure. i.e my_container.
You will get it if you know one of the field in the 'structure container'


**Reference:**

https://stackoverflow.com/questions/15832301/understanding-container-of-macro-in-the-linux-kernel
