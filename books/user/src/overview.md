# What is Cuprate?

Cuprate is an alternative implementation of a <a href="https://getmonero.org">Monero</a> node, designed to be a building block for the Monero network. Think of a Monero node as a crucial piece of software that helps maintain the network by verifying transactions and keeping a copy of the blockchain. While the original Monero node software, called `monerod` (or "Monero daemon"), is written in C++, Cuprate is built using the <a href="https://www.rust-lang.org/">Rust</a> programming language. This new daemon is known as `cuprated`.

Here are some key improvements and differences that Cuprate brings:

*   **Improved Safety**: Rust is known for its memory safety features, which can help prevent crashes and issues that might occur in C++ code. This means Cuprate may offer a more reliable and secure experience compared to monerod.
*   **Modern Architecture:** Cuprate is designed with a modern architecture that can be easier to maintain and extend. 
*   **Modularity:** Cuprate is built using Rust "crates", which means it's built with independent parts that interact with each other. This makes it easier for developers to fix issues. 
*   **Clear Documentation:** Cuprate will build extensive documentation, which explains how it works from the ground up. This makes it easier for new developers to contribute in the future.
*   **Benchmarking**: Cuprate has a built-in benchmarking system for testing and improving its performance. This ensures that it's not just safe but also efficient.

## An Example Use Case

Wallet software is a good user facing example of how Cuprate can improve the experience of using the Monero network. Let's think of your Monero wallet app as a house, and the software that powers it is like the foundation of that house. Currently, many wallets use `monerod` as their foundation, which is built with older materials (C++ code). `cuprated` is like a new, more advanced foundation built with modern materials (Rust code). This new foundation has several potential advantages:

*   **More Stable:** Rust is known for being very careful with how it manages resources. This means there's a good chance your wallet will have fewer crashes and general performance issues. It’s like having a house with a very solid foundation, ensuring the house stands firm.

*   **Faster and More Efficient:** The new "foundation" is designed to be fast and efficient. This means a Monero wallet could feel more responsive, like opening up quicker, processing transactions faster, and syncing more rapidly with the Monero network.

*   **Customizable Structure:** Cuprate’s communication system (RPC interface) can be adjusted and customized. This means that wallet developers could tweak it to improve performance, security, or add special features that users might like, such as storing recently used blocks. It's like having a house with a foundation that can be modified and customized to add new rooms or other features.

*   **Choice of Storage Materials:** Cuprate lets developers choose different ways to store your wallet's data, such as using either `heed` or `redb`. They can choose the one that's best for their app's needs. It’s like being able to choose the best type of material for your house’s foundation based on its needs and local environment.

*   **Adjustable Data Protection:** Cuprate allows wallet apps to choose how carefully they save your data to the computer's hard drive. A user with a fast computer might choose to save data quickly, whereas a user on an older computer might choose a safer method that is slightly slower, making sure no data is lost. 

Cuprate is not a user facing app itself (like the wallet example above). It's an underlying technology that Monero devlopers can use, and it is meant to be an alternative to `monerod` - not a replacement. All these improvements aim to help developers build better and more reliable Monero software by relying on `cuprated` instead of the older `monerod` software. The end result is a smoother and more secure experience for you even if you never directly interact with Cuprate.


