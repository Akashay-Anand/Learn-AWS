# Storage on AWS
> AWS storage services are grouped into three different categories: 
> - block storage
> - file storage
> - object storage.

## File Storage
> similar to the storage structure in our devices (pc, phone, etc).
>
> We place our files in a tree-like hierarchy that consists of folders and subfolders

> File storage is ideal when you require centralized access to files that need to be easily shared and managed by multiple host computers

> Common use cases for file storage include:
- Large content repositories
- Development environments
- User home directories

## Block Storage

> While file storage treats files as a singular unit, block storage splits files into fixed-size chunks of data called blocks that have their own addresses. Since each block is addressable, blocks can be retrieved efficiently.


> ![Alt text](/assets/storage_01.png)
> 
> in block storage we can easily modify small unit of data but in object storage we need to modify complete file.
> 
> This ease of access is why block storage solutions are **fast and use less bandwidth**. 

## Object Storage

> Objects, much like files, are also treated as a single unit of data when stored. However, unlike file storage, these objects are stored in a flat structure instead of a hierarchy. Each object is a file with a unique identifier. 
>
> Changing just one character in an object is more difficult than with block storage. When you want to change one character in a file, the entire file must be updated.
>
- benefits
  
> With object storage, you can store almost any type of data, and there is no limit to the number of objects stored, making it easy to scale
> 
> Object storage is generally useful when storing large data sets, unstructured files like media assets, and static assets, such as photos.