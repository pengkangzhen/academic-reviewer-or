# Academic Reviewer - Operations Research

A Claude Code Skill for critical academic review of Operations Research, Supply Chain, and Logistics papers targeting top-tier journals.

## Features

- **Mathematical Model Critique** - Novelty assessment, literature positioning, model validity
- **Algorithmic Contribution Assessment** - Incremental vs. significant advances, theoretical grounding
- **Numerical Experiment Evaluation** - Test instance design, benchmark selection, statistical rigor
- **Domain-Specific Expertise** - Stochastic programming, PHA/decomposition, maritime logistics

## Target Journals

- Operations Research (OR)
- Management Science (MS)
- Transportation Science (TS)
- Production and Operations Management (POM)
- European Journal of Operational Research (EJOR)
- Similar top-tier OR/Logistics venues

## Installation

### Method 1: Manual Installation

```bash
# Create skills directory if not exists
mkdir -p ~/.claude/skills/academic-reviewer-or

# Copy the SKILL.md file
cp skills/academic-reviewer-or/SKILL.md ~/.claude/skills/academic-reviewer-or/
```

### Method 2: Clone and Link

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/academic-reviewer-or.git
cd academic-reviewer-or

# Create symbolic link
mkdir -p ~/.claude/skills
ln -s $(pwd)/skills/academic-reviewer-or ~/.claude/skills/
```

## Usage

In Claude Code, invoke the skill:

```
/academic-reviewer-or
```

Then provide your code, model, or experimental results for review.

### Example

```
/academic-reviewer-or

I've implemented a Progressive Hedging Algorithm variant with adaptive penalty updates.
Here are my convergence results comparing to standard PHA...

[Your code and results]
```

## Review Output

The skill provides structured feedback:

- **Overall Assessment** - Publication potential (Strong/Acceptable/Weak/Reject)
- **Critical Issues** - Must address before submission
- **Moderate Issues** - Should address for stronger paper
- **Minor Issues** - Polish suggestions
- **Recommendations** - Concrete next steps

## Specialized Checks

### For Stochastic Programming
- VSS (Value of Stochastic Solution) analysis
- EVPI (Expected Value of Perfect Information)
- Scenario generation methodology
- Solution stability tests

### For Decomposition Algorithms (PHA, etc.)
- Penalty parameter justification
- Convergence criteria
- Comparison against DEP (Deterministic Equivalent Problem)
- Primal/dual residual tracking

### For Maritime/Container Logistics
- Real-world motivation
- Realistic parameter values
- Practical constraint modeling

## Requirements

- Claude Code CLI
- Claude Opus model recommended for best results

## License

MIT License - see [LICENSE](LICENSE)

## Contributing

Issues and pull requests welcome!

## Acknowledgments

Designed for researchers in Operations Research, Supply Chain Management, and Maritime Logistics.
