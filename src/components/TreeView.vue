<template>
    <div>
      <h2>{{ treeData.name }}</h2>
      <ul>
        <tree-node :node="treeData"></tree-node>
      </ul>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  import TreeNode from './TreeNode.vue'; // Import the TreeNode component
  
  const treeData = ref({
    name: 'GemmaForSequenceClassification',
    children: [
      {
        name: 'model',
        children: [
          {
            name: 'GemmaModel',
            children: [
              {
                name: 'embed_tokens',
                children: [
                  {
                    name: 'Embedding'
                  }
                ]
              },
              {
                name: 'layers',
                children: [
                  {
                    name: 'ModuleList',
                    children: [
                      {
                        name: '0-17',
                        count: 18,
                        children: [
                          {
                            name: 'GemmaDecoderLayer',
                            children: [
                              {
                                name: 'self_attn',
                                children: [
                                  {
                                    name: 'GemmaSdpaAttention',
                                    children: [
                                      {
                                        name: 'q_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'k_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'v_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'o_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'rotary_emb',
                                        children: [
                                          {
                                            name: 'GemmaRotaryEmbedding'
                                          }
                                        ]
                                      }
                                    ]
                                  }
                                ]
                              },
                              {
                                name: 'mlp',
                                children: [
                                  {
                                    name: 'GemmaMLP',
                                    children: [
                                      {
                                        name: 'gate_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'up_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'down_proj',
                                        children: [
                                          {
                                            name: 'Linear'
                                          }
                                        ]
                                      },
                                      {
                                        name: 'act_fn',
                                        children: [
                                          {
                                            name: 'PytorchGELUTanh'
                                          }
                                        ]
                                      }
                                    ]
                                  }
                                ]
                              },
                              {
                                name: 'input_layernorm',
                                children: [
                                  {
                                    name: 'GemmaRMSNorm'
                                  }
                                ]
                              },
                              {
                                name: 'post_attnetion_layernorm',
                                children: [
                                  {
                                    name: 'GemmaRMSNorm'
                                  }
                                ]
                              }
                            ]
                          }
                        ]
                      }
                    ]
                  }
                ]
              },
              {
                name: 'norm',
                children: [
                  {
                    name: 'GemmaRMSNorm'
                  }
                ]
              }
            ]
          }
        ]
      },
      {
        name: 'score',
        children: [
          {
            name: 'Linear'
          }
        ]
      }
    ]
  });
  </script>
  
  <style scoped>
  /* Your component styles here */
  </style>
  