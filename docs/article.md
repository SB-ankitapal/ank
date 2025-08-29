---
stoplight-id: fk66yvfwc23hv
internal: true
---

# article

The beginning of an awesome article...ggg
bnvhbhhbh
'some/text'
jnjnj
There is testing..jhjh

**t nest##test**
@#$test$#$%%
mnkn
\*\*_hi the re is testing_jhjmkff
frfff
~~hjkl; kjkjk~~
bnvnbhhjnjjmhj
> this is the quote.jhbgjhjbjmbhjbjgjhg mnbmknjnkmnjkn
mnmnmdfbj
[Google](https://meta.stoplight.io/docs/stoplight-api-docs/f6hiiufckkwgf-catalog-api-overview)

# management1

## management2gfhgnbnjknjbn

### management3

#### management4

##### management5

###### management6

`5677788890000000000899989`local model.  below are json

```
{
  "swagger": "2.0",
  "info": {
    "title": "2.0J",
    "version": "1.0"
  },
  "host": "localhost:3000",
  "basePath": "/",
  "schemes": [
    "http"
  ],
  "paths": {
    "/users/{userId}": {
      "get": {
        "summary": "Get User Info by User ID",
        "description": "Retrieve the information of the user with the matching user ID.",
        "operationId": "get-users-userId",
        "produces": [
          "application/json"
        ],
        "parameters": [
          {
            "name": "userId",
            "in": "path",
            "description": "Id of an existing user.",
            "required": true,
            "type": "integer"
          }
        ],
        "schemes": [
          "http"
        ],
        "responses": {
          "200": {
            "description": "User Found",
            "schema": {
              "type": "object",
              "properties": {
                "gujhu": {
                  "type": "number"
                },
                "sdscf": {},
                "dcccc": {
                  "type": "object",
                  "properties": {
                    "rfesf": {
                      "type": "array",
                      "items": {
                        "type": "array",
                        "items": {
                          "type": "array",
                          "items": {
                            "type": "array"
                          }
                        }
                      }
                    },
                    "fvvsv": {
                      "type": "object",
                      "properties": {
                        "dffvv": {
                          "type": "string"
                        },
                        "frfvvvds": {},
                        "fvfvvgg": {
                          "type": "object",
                          "properties": {
                            "freff": {
                              "type": "object",
                              "additionalProperties": {
                                "type": "array",
                                "items": {
                                  "type": "array",
                                  "items": {
                                    "type": "integer"
                                  }
                                }
                              }
                            },
                            "trgvv": {
                              "type": "string"
                            },
                            "rffvvgv": {
                              "type": "object",
                              "properties": {
                                "vvgvrf": {},
                                "SQWWSD": {
                                  "type": "object",
                                  "properties": {
                                    "VSCV": {},
                                    "VVT": {
                                      "type": "string"
                                    },
                                    "FVGVDV": {
                                      "type": "object",
                                      "properties": {
                                        "SDFFs": {
                                          "type": "integer"
                                        },
                                        "sfrfv": {},
                                        "refmodel": {
                                          "$ref": "#/definitions/model2"
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          }
                        }
                      }
                    }
                  }
                }
              }
            },
            "examples": {
              "Get User Alice Smith": {
                "id": 142,
                "firstName": "Alice",
                "lastName": "Smith",
                "email": "alice.smith@gmail.com",
                "dateOfBirth": "1997-10-31",
                "emailVerified": true,
                "signUpDate": "2019-08-24"
              }
            }
          },
          "404": {
            "description": "User Not Found",
            "schema": {
              "x-nullable": true
            }
          }
        }
      },
      "patch": {
        "summary": "Update User Information",
        "description": "Update the information of an existing user.",
        "operationId": "patch-users-userId",
        "produces": [
          "application/json"
        ],
        "consumes": [
          "application/json"
        ],
        "parameters": [
          {
            "name": "userId",
            "in": "path",
            "description": "Id of an existing user.",
            "required": true,
            "type": "integer"
          },
          {
            "in": "body",
            "name": "body",
            "schema": {
              "type": "object",
              "properties": {
                "firstName": {
                  "type": "string"
                },
                "lastName": {
                  "type": "string"
                },
                "email": {
                  "type": "string",
                  "description": "If a new email is given, the user's email verified property will be set to false."
                },
                "dateOfBirth": {
                  "type": "string"
                }
              }
            },
            "description": "Patch user properties to update."
          }
        ],
        "schemes": [
          "http"
        ],
        "responses": {
          "200": {
            "description": "User Updated",
            "schema": {
              "$ref": "#/definitions/User"
            },
            "examples": {
              "Update User Rebecca Baker": {
                "id": 13,
                "firstName": "Rebecca",
                "lastName": "Baker",
                "email": "rebecca@gmail.com",
                "dateOfBirth": "1985-10-02",
                "emailVerified": false,
                "createDate": "2019-08-24"
              }
            }
          },
          "404": {
            "description": "User Not Found",
            "schema": {
              "x-nullable": true
            }
          },
          "409": {
            "description": "Email Already Taken",
            "schema": {
              "x-nullable": true
            }
          }
        }
      }
    },
    "/user": {
      "post": {
        "summary": "Create New User",
        "description": "Create a new user.",
        "operationId": "post-user",
        "produces": [
          "application/json"
        ],
        "consumes": [
          "application/json"
        ],
        "parameters": [
          {
            "in": "body",
            "name": "body",
            "schema": {
              "type": "object",
              "properties": {
                "firstName": {
                  "type": "string"
                },
                "lastName": {
                  "type": "string"
                },
                "email": {
                  "type": "string"
                },
                "dateOfBirth": {
                  "type": "string",
                  "format": "date"
                }
              },
              "required": [
                "firstName",
                "lastName",
                "email",
                "dateOfBirth"
              ]
            },
            "description": "Post the necessary fields for the API to create a new user."
          }
        ],
        "schemes": [
          "http"
        ],
        "responses": {
          "200": {
            "description": "User Created",
            "schema": {
              "$ref": "#/definitions/User"
            }
          },
          "400": {
            "description": "Missing Required Information",
            "schema": {
              "x-nullable": true
            }
          },
          "409": {
            "description": "Email Already Taken",
            "schema": {
              "x-nullable": true
            }
          }
        }
      }
    }
  },
  "definitions": {
    "model2": {
      "type": "object",
      "title": "model2",
      "description": "model1",
      "properties": {
        "id": {
          "type": "number"
        },
        "dexter": {
          "type": "array",
          "items": {
            "type": "array",
            "items": {
              "type": "array",
              "items": {
                "type": "array",
                "items": {
                  "type": "array"
                }
              }
            }
          }
        },
        "didi": {},
        "Tramp": {
          "type": "boolean"
        },
        "refermodel1": {
          "$ref": "#/definitions/Model1"
        }
      }
    },
    "Model1": {
      "type": "object",
      "title": "Model1",
      "description": "model1",
      "properties": {
        "id": {
          "type": "string"
        },
        "Tom": {
          "type": "boolean"
        },
        "Jerry": {},
        "scooby": {
          "type": "object",
          "additionalProperties": {
            "type": "number"
          }
        }
      }
    },
    "User": {
      "type": "object",
      "title": "User",
      "properties": {
        "id": {
          "type": "integer",
          "description": "Unique identifier for the given user."
        },
        "firstName": {
          "type": "string"
        },
        "lastName": {
          "type": "string"
        },
        "email": {
          "type": "string",
          "format": "email"
        },
        "dateOfBirth": {
          "type": "string",
          "format": "date",
          "x-examples": [
            "1997-10-31"
          ]
        },
        "emailVerified": {
          "type": "boolean",
          "description": "Set to true if the user's email has been verified."
        },
        "createDate": {
          "type": "string",
          "description": "The date that the user was created.",
          "format": "date"
        }
      },
      "required": [
        "id",
        "firstName",
        "lastName",
        "email",
        "emailVerified"
      ]
    }
  }
}







```

1. testing

- the process
- \[check] the teams call

| Column A | Column B | Column C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3       |

| Column A | Column B | Column C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3test   |

```json http
{
  "method": "get",
  "url": "https://todos.stoplight.io/todos"
}
```

```json jsonSchema
{
  "type": "object",
  "properties": {
    "id": {
      "type": "string"
    }
  }
}
```

![image (49).png](<../assets/images/image (49).png>)
