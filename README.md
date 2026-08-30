# LUFFY Development Repository

> 🚧 **Development Branch** - This is the main development repository for LUFFY (Learning to Reason Under Off‑Policy Guidance)

## About LUFFY

LUFFY is a reinforcement learning framework that bridges the gap between zero-RL and imitation learning by incorporating off-policy reasoning traces into the training process. This repository contains the core implementation and development work.

## 🔧 Development 

This branch contains active development code. The code in this repository is under active development and may not be stable. Please refer to the main branch for stable releases.

## Current Development Focus

### API Integration
- **OpenAI API**: Client initialization, authentication, retry logic, error handling, and response parsing are implemented.
- **Gemini API**: Still needs completion.

### Data Processing
- **Core batch dimension folding/unfolding**: Implemented.
- **Remaining optimization items**: Still tracked as TODOs.

## 📝 Complete TODO List
- [x] **luffy/deepscaler/utils.py:45** - Implement OpenAI API client initialization
- [x] **luffy/deepscaler/utils.py:46** - Add proper authentication handling
- [x] **luffy/deepscaler/utils.py:47** - Implement exponential backoff retry logic for rate limits
- [x] **luffy/deepscaler/utils.py:48** - Add comprehensive error handling for different API errors
- [x] **luffy/deepscaler/utils.py:49** - Implement response parsing and validation
- [ ] **luffy/deepscaler/utils.py:50** - Implement Gemini API client initialization
- [ ] **luffy/deepscaler/utils.py:51** - Add Gemini-specific authentication
- [ ] **luffy/deepscaler/utils.py:52** - Handle Gemini API rate limiting
- [ ] **luffy/deepscaler/utils.py:53** - Add Gemini API error handling
- [ ] **luffy/deepscaler/utils.py:54** - Parse Gemini API responses
- [ ] **luffy/verl/verl/protocol.py:132** - Add support for variable batch dimensions
- [ ] **luffy/verl/verl/protocol.py:133** - Optimize tensor view operations for performance
- [ ] **luffy/verl/verl/protocol.py:134** - Handle non-tensor batch data reshaping properly
- [ ] **luffy/verl/verl/protocol.py:135** - Add error handling for invalid batch dimensions
- [ ] **luffy/verl/verl/protocol.py:156** - (zhangchi.usc1992) add consistency check
- [ ] **luffy/verl/verl/protocol.py:252** - we can actually lift this restriction if needed
- [ ] **luffy/verl/verl/protocol.py:338** - (zhangchi.usc1992) whether to copy

## How to Contribute
1. Pick a TODO item
2. Implement the functionality
3. Test your implementation
4. Update this README when TODOs are completed
