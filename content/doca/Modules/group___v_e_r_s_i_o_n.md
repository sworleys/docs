---
title: Version Management

---

# Version Management

 [More...](#detailed-description)

## Functions

|                | Name           |
| -------------- | -------------- |
| const char * | **[doca_version](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#function-doca_version)**(void )<br>Function returning version string.  |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[DOCA_VER_MAJOR](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_major)** <br>Major version number 0-255.  |
|  | **[DOCA_VER_MINOR](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_minor)** <br>Minor version number 0-255.  |
|  | **[DOCA_VER_PATCH](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_patch)** <br>Patch version number 0-255.  |
|  | **[DOCA_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_num)**(major, minor, patch) <br>Macro of version number for comparisons.  |
|  | **[DOCA_CURRENT_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_current_version_num)** <br>Macro of current version number for comparisons.  |
|  | **[DOCA_VERSION_EQ_CURRENT](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_eq_current)**(major, minor, patch) <br>Return 1 if the version specified is equal to current.  |
|  | **[DOCA_VERSION_LTE_CURRENT](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_lte_current)**(major, minor, patch) <br>Return 1 if the version specified is less then or equal to current.  |

## Detailed Description


Define function to get doca version and version compare. 


## Functions Documentation

### function doca_version

```cpp
static inline const char * doca_version(
    void 
)
```

Function returning version string. 

**Return**: string version number of a format major.minor.patch 



## Macros Documentation

### define DOCA_VER_MAJOR

```cpp
#define DOCA_VER_MAJOR 0
```

Major version number 0-255. 

### define DOCA_VER_MINOR

```cpp
#define DOCA_VER_MINOR 1
```

Minor version number 0-255. 

### define DOCA_VER_PATCH

```cpp
#define DOCA_VER_PATCH 0
```

Patch version number 0-255. 

### define DOCA_VERSION_NUM

```cpp
#define DOCA_VERSION_NUM(
    major,
    minor,
    patch
)
((major) << 16 | (minor) << 8 | (patch))
```

Macro of version number for comparisons. 

### define DOCA_CURRENT_VERSION_NUM

```cpp
#define DOCA_CURRENT_VERSION_NUM [DOCA_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_num)([DOCA_VER_MAJOR](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_major), [DOCA_VER_MINOR](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_minor), [DOCA_VER_PATCH](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_ver_patch))
```

Macro of current version number for comparisons. 

### define DOCA_VERSION_EQ_CURRENT

```cpp
#define DOCA_VERSION_EQ_CURRENT(
    major,
    minor,
    patch
)
	([DOCA_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_num)(major, minor, patch) == [DOCA_CURRENT_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_current_version_num))
```

Return 1 if the version specified is equal to current. 

### define DOCA_VERSION_LTE_CURRENT

```cpp
#define DOCA_VERSION_LTE_CURRENT(
    major,
    minor,
    patch
)
	([DOCA_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_version_num)(major, minor, patch) <= [DOCA_CURRENT_VERSION_NUM](localhost:1313/networking-ethernet-software/doca/modules/group___v_e_r_s_i_o_n/#define-doca_current_version_num))
```

Return 1 if the version specified is less then or equal to current. 



-------------------------------

Updated on  2 August 2021 at 20:00:04 EDT