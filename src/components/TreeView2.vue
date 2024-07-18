<template>
    <div>
      <v-network-graph :nodes="nodes" :edges="edges"></v-network-graph>
      <nodeTree/>
    </div>
  </template>
  
  <script setup>
  import VNetworkGraph from 'v-network-graph';
  import 'v-network-graph/lib/style.css';
  
  // Define the converted nodeTree object
  const nodeTree = {
    GemmaForSequenceClassification: {
      id: "GemmaForSequenceClassification",
      name: "GemmaForSequenceClassification",
      collapse: false,
      children: {
        model: {
          id: "GemmaForSequenceClassification/model",
          name: "model",
          children: {
            GemmaModel: {
              id: "GemmaForSequenceClassification/model/GemmaModel",
              name: "GemmaModel",
              children: {
                embed_tokens: {
                  id: "GemmaForSequenceClassification/model/GemmaModel/embed_tokens",
                  name: "embed_tokens",
                  children: {
                    Embedding: {
                      id: "GemmaForSequenceClassification/model/GemmaModel/embed_tokens/Embedding",
                      name: "Embedding"
                    }
                  }
                },
                layers: {
                  id: "GemmaForSequenceClassification/model/GemmaModel/layers",
                  name: "layers",
                  children: {
                    ModuleList: {
                      id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList",
                      name: "ModuleList",
                      children: {
                        "0-17": {
                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17",
                          name: "0-17",
                          children: {
                            GemmaDecoderLayer: {
                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer",
                              name: "GemmaDecoderLayer",
                              children: {
                                self_attn: {
                                  id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn",
                                  name: "self_attn",
                                  children: {
                                    GemmaSdpaAttention: {
                                      id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention",
                                      name: "GemmaSdpaAttention",
                                      children: {
                                        q_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/q_proj",
                                          name: "q_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/q_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        k_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/k_proj",
                                          name: "k_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/k_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        v_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/v_proj",
                                          name: "v_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/v_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        o_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/o_proj",
                                          name: "o_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/o_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        rotary_emb: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/rotary_emb",
                                          name: "rotary_emb",
                                          children: {
                                            GemmaRotaryEmbedding: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/self_attn/GemmaSdpaAttention/rotary_emb/GemmaRotaryEmbedding",
                                              name: "GemmaRotaryEmbedding"
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                },
                                mlp: {
                                  id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp",
                                  name: "mlp",
                                  children: {
                                    GemmaMLP: {
                                      id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP",
                                      name: "GemmaMLP",
                                      children: {
                                        gate_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/gate_proj",
                                          name: "gate_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/gate_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        up_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/up_proj",
                                          name: "up_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/up_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        down_proj: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/down_proj",
                                          name: "down_proj",
                                          children: {
                                            Linear: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/down_proj/Linear",
                                              name: "Linear"
                                            }
                                          }
                                        },
                                        act_fn: {
                                          id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/act_fn",
                                          name: "act_fn",
                                          children: {
                                            PytorchGELUTanh: {
                                              id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/mlp/GemmaMLP/act_fn/PytorchGELUTanh",
                                              name: "PytorchGELUTanh"
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                },
                                input_layernorm: {
                                  id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/input_layernorm",
                                  name: "input_layernorm",
                                  children: {
                                    GemmaRMSNorm: {
                                      id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/input_layernorm/GemmaRMSNorm",
                                      name: "GemmaRMSNorm"
                                    }
                                  }
                                },
                                post_attnetion_layernorm: {
                                  id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/post_attnetion_layernorm",
                                  name: "post_attnetion_layernorm",
                                  children: {
                                    GemmaRMSNorm: {
                                      id: "GemmaForSequenceClassification/model/GemmaModel/layers/ModuleList/0-17/GemmaDecoderLayer/post_attnetion_layernorm/GemmaRMSNorm",
                                      name: "GemmaRMSNorm"
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
                norm: {
                  id: "GemmaForSequenceClassification/model/GemmaModel/norm",
                  name: "norm",
                  children: {
                    GemmaRMSNorm: {
                      id: "GemmaForSequenceClassification/model/GemmaModel/norm/GemmaRMSNorm",
                      name: "GemmaRMSNorm"
                    }
                  }
                }
              }
            }
          }
        }
      },
      score: {
        id: "GemmaForSequenceClassification/score",
        name: "score",
        children: {
          Linear: {
            id: "GemmaForSequenceClassification/score/Linear",
            name: "Linear"
          }
        }
      }
    }
  };
  
  // Function to convert the tree structure into nodes and edges
  function convertTreeToGraph(tree) {
    const nodes = [];
    const edges = [];
  
    function traverse(node, parentId = null) {
      const nodeId = node.id; // Use the provided id
      nodes.push({ id: nodeId, label: node.name });
  
      if (parentId !== null) {
        edges.push({ from: parentId, to: nodeId });
      }
  
      if (node.children) {
        Object.values(node.children).forEach(child => traverse(child, nodeId));
      }
    }
  
    Object.values(tree).forEach(group => traverse(group));
    
    return { nodes, edges };
  }
  
  const { nodes, edges } = convertTreeToGraph(nodeTree);
  
  </script>
  
  <style scoped>
  /* Your component styles here */
  </style>
  