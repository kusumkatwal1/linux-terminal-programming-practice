## Linux Filesystems and Storage Fundamentals:
      - A disk is not the same thing as a filesystem.
      - A filesystem is the structure Linux uses to organize data on storage.
      - Also, it keeps track of all the things.
      - Some important terms:
               - Disk: Storage device
               - Partition: Disk section
               - Filesystem: Organizes files
               - Mount point: Access directory
               - UUID: Unique filesystem ID
                          
      - Flow: Disk → Partition → Filesystem → Mount Point.
          
      - Some repetitive commands are listed below:
         
## Commands:
#### 1. pwd:
      - Shows your current working directory.

#### 2. ls:
      - Important for filesystem navigation.

#### 3. lsblk:
      - it specifically for storage investigation.

#### 4. blkid:
      - Identifies block devices and filesystem metadata.

#### 5. findmnt:
      - Shows mounted filesystems and their relationships.
      - Syntax: "findmnt".

#### 6. df and mount:
      - These are repetitive commands.
      - DF: Filesystem → Mount Point.
      - mount: Attaches a filesystem to a directory.

#### 7. umount:
      - Detaches a filesystem.

#### 8. tmpfs:
      - Linux can mount a filesystem backed primarily by memory.

## Cheat Code:
            pwd                         # Current directory
            ls -lah                     # List files
            lsblk                       # List block devices
            lsblk -f                    # Filesystem information
            sudo blkid                  # UUID and filesystem type
            findmnt                     # Show mounted filesystems
            findmnt /                   # Check a specific mount
            df -h                       # Disk usage
            df -i                       # Inode usage
            du -sh *                    # Directory usage
            du -xhd1 /                  # Root directory usage
            
            sudo mkdir -p /data         # Create mount point
            sudo mount /dev/sdb1 /data  # Mount filesystem
            sudo umount /data           # Unmount filesystem
            
            sudo lsof /data             # Find processes using mount
            sudo fuser -vm /data        # Find users/processes
            
            cat /etc/fstab              # View mount configuration
            sudo mount -a               # Test fstab
  


@kusum katwal
