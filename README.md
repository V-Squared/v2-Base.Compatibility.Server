# V-Base.Compatibility.Server

This is a rest+Nosql PHP implementation.  The goal of the project is to create a system logging tool.  This is the middlewear layer.
**V1.0 API overview**
 
**Objects**

·      
Record, represents one machine test

·      
Device, represents a device in a computer

**For Report page**

·      
/record/

o   Lists
all Records

·      
/record/(recordID)/device/

o   List
all devices under a record

**For Desktop App**

·      
GET /record/(recordID)/

o   Returns
a Record or creates a new one

·      
Get /record/(recordID)/device/(deviceID)/

o   Returns
a device for a record or creates a new device or creates new both

·      
POST /record/(recordID)/device/(deviceID)/

o   Saves
all Post Key/Value Pairs to a device, and/or creates record and device if
needed


**Database Technology:**

NoSQL Document Store – Objects are pushed into RedbeanPHP
and a database schema is created based on the objects and updated dynamically. 
