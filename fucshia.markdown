---
layout: single
author_profile: true
permalink: /fuchsia/
title: Fuchsia
---

# My Commits

```bash
git clone https://fuchsia.googlesource.com/fuchsia
cd fuchsia
git log --author=boetger@google.com 
```

Mostly focues on building the new developer tool: [FFX](https://fuchsia.dev/fuchsia-src/development/tools/ffx/overview)

commit aad819ab0f102eba452d100394a97d7149603b7e
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 29 16:56:48 2022 +0000

    [ffx] remove ssh-key param from ffx target flash
    
    Fixed: 94641, 83122
    Change-Id: Id7550900c8e979f73184ca32455d0f1f77c361ca
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/652402
    Fuchsia-Auto-Submit: Omer Lev-ran <omerlevran@google.com>
    Reviewed-by: Omer Lev-ran <omerlevran@google.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 271bb219ebb4fefdc1bb34c5e6b0e23e67831dcb
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 15 22:49:45 2022 +0000

    [ffx] Add more helpful error message when creating environment file
    
    Fixed: 93589
    Change-Id: I8fbc16dc2aee23beb749dba0f2b3d6b5855c519c
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/653089
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit 60e0c930a249b31dba565a1f06fb3bfc853c5ca4
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 15 16:55:05 2022 +0000

    [ffx] update calling scripts to use --authorized-keys
    
    Bug: 83122
    Change-Id: Ife031dbe5dc7593d5c2d5e65c9dc2f76b431e2b3
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/652185
    Reviewed-by: Omer Lev-ran <omerlevran@google.com>
    Reviewed-by: Renato Mangini Dias <mangini@google.com>
    Reviewed-by: Ina Huh <ihuh@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit b9dcff490f611362413844d4fdedb15496e1b154
Author: Matt Boetger <boetger@google.com>
Date:   Mon Mar 14 21:29:16 2022 +0000

    [ffx] better reboot errors for `ffx target flash`
    
    Fixed: 83751
    
    Change-Id: I3d6775a82925cdce3d0145407fffe1950f9d3717
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/649799
    Reviewed-by: Andrew Davies <awdavies@google.com>
    API-Review: Dave Schuyler <dschuyler@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit 85bcc1767de0351d23338966aa30045ebd1fcfe3
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 1 20:44:11 2022 +0000

    [ffx] Add authorized_keys param to `ffx target flash`
    
    Bug: 83122
    Change-Id: Icac3e5946607d46324611b19ee52c17b02e2f7a6
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/652242
    Fuchsia-Auto-Submit: Matt Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 9798476a7ca85f4852af118dc44add6969e8bed3
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 1 20:38:26 2022 +0000

    [ffx] Fix key mismatch error message
    
    Fixed: 91528
    Change-Id: I8b92b79fc265ca1afecf30dcb9b75c3830dd4031
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/652224
    Fuchsia-Auto-Submit: Matt Boetger <boetger@google.com>
    Reviewed-by: David Pursell <dpursell@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit b1f88d7cb185005f83ee7d9382e8f3fc9d7e8ec1
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 1 20:11:22 2022 +0000

    [ffx] Add helpful error messages for invalid environment file
    
    Fixed: 93589
    
    Change-Id: Ibe15e8b89ad86c5041bdd69348ce4aae5054c705
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/652223
    Fuchsia-Auto-Submit: Matt Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit c67846d8b3908571f38c83bdd29192c2073367be
Author: Matt Boetger <boetger@google.com>
Date:   Wed Feb 2 21:27:24 2022 +0000

    [ffx] Disabled zedboot discovery by default
    
    This creates a configuration key, "discovery.zedboot.enabled" that
    controls Zedboot discovery.  If a user wants to enable Zedboot
    discovery, they can run
    
    ffx config set discovery.zedboot.enabled true
    
    Fixed: 90219
    Change-Id: I6707fe5b7d8b0d5219f28111d329cd0f6447f1b1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/639821
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit 1faa00837584bbce7693a682336cd931b57a5681
Author: Matt Boetger <boetger@google.com>
Date:   Fri Dec 24 00:11:18 2021 +0000

    [ffx] fix `ffx target flash` not sending ssh keys
    
    Change-Id: Iba248acc626566d399de79ecf99487e4b287a42e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/624324
    Fuchsia-Auto-Submit: Matt Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Reviewed-by: Akira Baruah <akirabaruah@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 9de872343a73b8d8edfab84f89d19a5a9e08596d
Author: Matt Boetger <boetger@google.com>
Date:   Mon Dec 20 20:34:08 2021 +0000

    [ffx] add bootloader subcommand
    
    This creates a common library under ffx/lib because there are two
    commands now that use the common functionality:
    
    `ffx target flash`
    
    and
    
    `ffx target bootloader info/lock/unlock/boot`
    
    Fixed: 89897
    
    Change-Id: I2d648d5354311bce3367273224231d91b5feebb8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/617579
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit 048f7278cf099a4888d2bb53ced5697bb5778edd
Author: Matt Boetger <boetger@google.com>
Date:   Sat Dec 11 00:11:34 2021 +0000

    Reland "[build] Include gpt in default Fuchsia product"
    
    This reverts commit 3efbc81461db5d9ba37285a884b49bd5a3c1c1fe.
    
    Reason for revert: fxr/612420 should have fixed the issue with fx flash-remote
    
    Original change's description:
    > Revert "[build] Include gpt in default Fuchsia product"
    >
    > This reverts commit 74cd072b0ed5d25e2a3a78aeafdc3dd0e4c3d1e9.
    >
    > Reason for revert: Unlock credentials are not copied in `fx flash-remote`
    >
    > Original change's description:
    > > [build] Include gpt in default Fuchsia product
    > >
    > > In the flash manifest, include the gpt partitions in the default
    > > "fuchsia" product.  This will mean any users running `ffx target flash`
    > > will automatically get the benefit of re-flashing the gpt images without
    > > having to change scripts.
    > >
    > > Fixed: 88710
    > > Change-Id: Ifc6505086877dffdf17e4406372af4a348844399
    > > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/607121
    > > Reviewed-by: Aidan Wolter <awolter@google.com>
    > > Commit-Queue: Matthew Boetger <boetger@google.com>
    >
    > Change-Id: Ide0411f361fce16ccccd531dc87ae7df49efb2e8
    > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/609347
    > Reviewed-by: RubberStamper 🤖 <android-build-ayeaye@system.gserviceaccount.com>
    > Commit-Queue: Matthew Boetger <boetger@google.com>
    
    Change-Id: I361521ea866e82823f5bd6dbe4481b0b57bc68ff
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/615199
    Reviewed-by: Aidan Wolter <awolter@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit e6ed3890f10fbcc4a2c2b724cfb2f55f24fbfe4b
Author: Matt Boetger <boetger@google.com>
Date:   Wed Dec 8 20:45:31 2021 +0000

    [ffx] create `ffx sdk list` command
    
    Change-Id: I9f21ac5370c2544a439369fccc01d26e9329ed24
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/613023
    Reviewed-by: Dave Schuyler <dschuyler@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit d6fd4c391fd4215b9e6c61035c179413c845d889
Author: Matt Boetger <boetger@google.com>
Date:   Tue Dec 7 19:21:55 2021 +0000

    [ffx] add gcs downloading to `ffx target flash`
    
    Change-Id: I2fe432d97edcdaf52503617a07bb06728165de86
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/610376
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Dave Schuyler <dschuyler@google.com>
    Commit-Queue: Matt Boetger <boetger@google.com>

commit 59439847a72a491bbc551577284f1db54383bd6d
Author: Matt Boetger <boetger@google.com>
Date:   Mon Dec 6 22:24:05 2021 +0000

    [ffx] add `ffx target flash info`
    
    Should print all the fastboot variables.
    
    Fixed: 89561
    Change-Id: I474d9188d6c2662b5994d8096d53ebe2a35072a2
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/612136
    Fuchsia-Auto-Submit: Matt Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit ed673a1bddfd2491c6ad4e32e4af40d58047c3d7
Author: Matt Boetger <boetger@google.com>
Date:   Thu Dec 2 23:06:57 2021 +0000

    [ffx] Fix `ffx config env set` command
    
    Bug: 81502
    Change-Id: I3f09aa061964e99496d9a856c70a3e756144a0f5
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/612821
    Commit-Queue: Matt Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>

commit fe1f05aa30c4b828f3335f20328256a338a6b412
Author: Matt Boetger <boetger@google.com>
Date:   Wed Nov 24 00:45:45 2021 +0000

    [ffx] `ffx target flash boot` subcommand
    
    Change-Id: Ia4d3df2f4b241ce3ca2cfdaa39601e2b40908f0f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/606645
    Reviewed-by: Andrew Davies <awdavies@google.com>
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 3efbc81461db5d9ba37285a884b49bd5a3c1c1fe
Author: Matthew Boetger <boetger@google.com>
Date:   Fri Nov 19 21:50:05 2021 +0000

    Revert "[build] Include gpt in default Fuchsia product"
    
    This reverts commit 74cd072b0ed5d25e2a3a78aeafdc3dd0e4c3d1e9.
    
    Reason for revert: Unlock credentials are not copied in `fx flash-remote`
    
    Original change's description:
    > [build] Include gpt in default Fuchsia product
    >
    > In the flash manifest, include the gpt partitions in the default
    > "fuchsia" product.  This will mean any users running `ffx target flash`
    > will automatically get the benefit of re-flashing the gpt images without
    > having to change scripts.
    >
    > Fixed: 88710
    > Change-Id: Ifc6505086877dffdf17e4406372af4a348844399
    > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/607121
    > Reviewed-by: Aidan Wolter <awolter@google.com>
    > Commit-Queue: Matthew Boetger <boetger@google.com>
    
    Change-Id: Ide0411f361fce16ccccd531dc87ae7df49efb2e8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/609347
    Reviewed-by: RubberStamper 🤖 <android-build-ayeaye@system.gserviceaccount.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 1811067ca08e2aa4384c82fe1b32e83677a77c2f
Author: Matt Boetger <boetger@google.com>
Date:   Wed Nov 17 20:38:38 2021 +0000

    [ffx] Unlock subcommand for `ffx target flash`
    
    Allows users to unlock fastboot targets.
    
    Change-Id: I88b752113c7a23cb958f2330f5a3ca4bb01c627d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/605672
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 55e6c44854e183b84edb697f16a102e586271786
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 16 22:42:34 2021 +0000

    [ffx] Remove common library in favor of single plugin
    
    Sorry for the churn, but since FfxConfigBacked only works on top level
    argh params, it makes more sense to just treat this as one plugin and
    route the subcommands manually.  This prevents a strange dependency
    graph as the subcommands will need access to the manifest parameter on
    the parent subcommand.
    
    Change-Id: I2b81bebdf1cdf33ce729f99d3ffd77282397a18b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/605521
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit b162bc709a8b0da378d81e3cbdcf322c5db56d1b
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 16 19:13:22 2021 +0000

    [ffx] add ffx target flash lock plugin
    
    Change-Id: Ia7a68805e9e796954b4847daa343483433de8a33
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/604998
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 2fcf507fe1a8f8e11eea2d4f34993abdf4c16462
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 16 17:41:59 2021 +0000

    [ffx] Check full name too to verify hardware
    
    Bug: 88373
    Change-Id: Ia183a77347451d5545aaaf3a67c6825eeccb742b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/607126
    Reviewed-by: David Pursell <dpursell@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 74cd072b0ed5d25e2a3a78aeafdc3dd0e4c3d1e9
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 16 01:32:32 2021 +0000

    [build] Include gpt in default Fuchsia product
    
    In the flash manifest, include the gpt partitions in the default
    "fuchsia" product.  This will mean any users running `ffx target flash`
    will automatically get the benefit of re-flashing the gpt images without
    having to change scripts.
    
    Fixed: 88710
    Change-Id: Ifc6505086877dffdf17e4406372af4a348844399
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/607121
    Reviewed-by: Aidan Wolter <awolter@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 4717c2f9269b3e9b2548f6b33c54468b09acacc5
Author: Matt Boetger <boetger@google.com>
Date:   Mon Nov 15 20:29:17 2021 +0000

    [ffx] Add config key to disable usb enumeration
    
    Fixed: 87441
    Change-Id: I189f759ce585cda6621668524af2cf4174221ce1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/604485
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 56e6f231f437016d811c44045d1ea3f2e0a717a7
Author: Matt Boetger <boetger@google.com>
Date:   Thu Nov 11 09:09:19 2021 +0000

    [ffx] fastboot common library
    
    This creates a common library that can be shared between subcommands of
    `ffx target flash`.  This is in preparation for `ffx target flash boot`,
    `ffx target flash lock`, and `ffx target flash unlock`.
    
    Fixed: 86760
    
    Change-Id: I60582d9784d69d83d253406b0279fcd54277d146
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/594014
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>

commit c6669f0169251c523969a0eaf4273be329832f00
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 27 23:58:51 2021 +0000

    [ffx] Update proxy map for `ffx target show`
    
    Change-Id: Ifaea184ae9be18b9f70038265a3a86f15ba8117a
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/598609
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Amit Uttamchandani <amituttam@google.com>
    Fuchsia-Auto-Submit: Amit Uttamchandani <amituttam@google.com>

commit 33a601ffff07010508f8a956841ca4070496a57f
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 27 20:06:12 2021 +0000

    [ffx] Re-lock the device after bootloader parts
    
    Locking the device deletes the SSH keys, so make sure we lock before
    staging the SSH keys.
    
    Change-Id: Ic35a809553666fd92ea34e3d5afd014d17b615c7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/595444
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 41929cecf5239b48a76ac70ce131f77a44cd35c5
Author: Matt Boetger <boetger@google.com>
Date:   Mon Oct 18 19:34:56 2021 +0000

    [ffx] Generate the unlock token and unlock a device.
    
    Fixed: 85902, 85903
    Change-Id: I926d3f275f0bc790da797203efd323df7ad967de
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/591300
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 3779f2bcd24cc1cb5c347eb68da90bee4b4e722e
Author: Matt Boetger <boetger@google.com>
Date:   Thu Oct 14 19:48:52 2021 +0000

    [ffx] Match credentials file to device
    
    Fixed: 85901
    
    Change-Id: Id1a7f99ecaebb0984cca710de330b2d8ac6ed100
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/591506
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 9f2c39766a25b70890c948f3847dfbb710516f4f
Author: Matthew Boetger <boetger@google.com>
Date:   Wed Oct 13 21:43:35 2021 +0000

    [ffx] Revert breaking changes in main.rs
    
    Also revert changes to `ffx target show`.  Without the change to
    main.rs, the fastboot solution in ffx target show will be unusable.
    
    Change-Id: I4a04ca125afd528d636c05bf3395d0478fbff864
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/592782
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 41896c1580afed72a316654cbdf9be35a628322f
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 13 18:44:25 2021 +0000

    [ffx] Get the unlock challenge from the device
    
    Download the data for the unlock challenge from a fastboot device.
    
    Bug: 85901
    
    Change-Id: Ic135dd5eefd495f629fa4c9c00ac1a7b7628a472
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/590914
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 7a5659579e2340a50cbd5063ee7925b46d4fcf6f
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 8 23:40:26 2021 +0000

    [ffx] Abstract out flashing logic between versions.
    
    Since unlocking logic is different from v1 and v2, and it's internal to
    the product, some of the flashing logic needs to be abstracted out in
    order create space for unlocking logic.
    
    Bug: 85901
    Change-Id: Ie7aa37c046f9a48694f7170a4b21026f44af4cd7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/590388
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 5ca97c0fb895df216ba5072f103ba26cf5f84d14
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 8 23:11:57 2021 +0000

    [ffx][images] Remove bootstrap product if no bootstrap_files
    
    Change-Id: Ie8eacd3d634d24252a3aab93dfeed8943e795946
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/591368
    Reviewed-by: David Pursell <dpursell@google.com>
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit d0daacae9375a535324dcf7c0350985b995e0df4
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 8 20:04:45 2021 +0000

    [ffx] Add credentials to the FFX manifest.
    
    Need to add unlocking credentials to the flash manifest.
    
    Bug: 85901
    Change-Id: Iaebe64c44289c01198aae4449653342898741894
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/590263
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 0368f3f843b61ad0e60126bb2b48fed2acd3b16e
Author: Matt Boetger <boetger@google.com>
Date:   Mon Oct 4 23:03:25 2021 +0000

    [ffx] Add unlock_creds field to flash manifest.
    
    Bug: 84916
    
    Change-Id: Ic43b6c66cfc36ab085d3622fd889f8dcaf3e2b58
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/586169
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Misha Gridnev <gridman@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Reviewed-by: David Pursell <dpursell@google.com>

commit 15b13c190fab5c545fa59ecc72a9c264c512f36b
Author: Matt Boetger <boetger@google.com>
Date:   Mon Oct 4 18:35:02 2021 +0000

    [ffx] Add requires_unlock to flash manifest
    
    Change-Id: I6f4185a44eac1fd784c004c8281f78b747c3ab15
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/587861
    Reviewed-by: Misha Gridnev <gridman@google.com>
    Reviewed-by: David Pursell <dpursell@google.com>
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Reviewed-by: Omer Lev-ran <omerlevran@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 0c5b9438deda03621f5035180465853a36646c59
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 1 00:19:43 2021 +0000

    [ffx] Add fastboot proxy to `ffx target show`
    
    This also makes sure the remote control proxy is only tried once despite
    having multiple proxies.
    
    Fixed: 78881,84858
    Change-Id: I7f80f8f78232dbbdfe826e5dedcfcc5df933d268
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/585181
    Reviewed-by: Dave Schuyler <dschuyler@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    API-Review: Dave Schuyler <dschuyler@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 73d982905aae0c5bc07925229366ff641f31710b
Author: Matt Boetger <boetger@google.com>
Date:   Thu Sep 30 19:07:52 2021 +0000

    [ffx] Add requires_unlock field to V3
    
    The bootstrap product will need to be marked with this field to identify
    that in order to succeed, the device will need to be unlocked.  If the
    device is not unlocked, then an error message is shown.
    
    Change-Id: I727e26e231d635719a6b089c0797c620851ed5d4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/586170
    Reviewed-by: David Pursell <dpursell@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 9036564798e5a4bd06f990fce09297c004d2abd6
Author: Matt Boetger <boetger@google.com>
Date:   Fri Sep 17 01:24:01 2021 +0000

    [ffx] Remove unnecessary `mod args` in assembly
    
    Plugins should be getting their args from the plugin args library and
    not double including the args.rs file. This should help incremental
    builds.
    
    Change-Id: I19086c95855628bd74fe7093a61c11a38b8d5039
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/582005
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit cd43d800aab6855ef3727cca07efc621ae9c976e
Author: Matt Boetger <boetger@google.com>
Date:   Thu Sep 16 00:45:57 2021 +0000

    [ffx] Extends args_sources to rest of plugins
    
    Change-Id: I9ca5b69187bcc5ef19f38f43baff2fad20bfb384
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/581516
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit b0795d26b6a99afd5bbaf10a6904246e396d6f3d
Author: Matt Boetger <boetger@google.com>
Date:   Wed Sep 15 23:06:19 2021 +0000

    [ffx] Use args_sources in full target chain
    
    Propagating the args_sources property up the entire `ffx target` chain
    helps with performance a little bit more.
    
    Tested:
    
    Before:
    
    ╰─❯ time fx build ffx
    ninja: Entering directory `/Users/boetger/fuchsia/out/default'
    [29/29] STAMP obj/src/developer/ffx/ffx.stamp
    fx build ffx  159.49s user 6.27s system 134% cpu 2:02.98 total
    
    After:
    
    ╰─❯ time fx build ffx
    ninja: Entering directory `/Users/boetger/fuchsia/out/default'
    [29/29] STAMP obj/src/developer/ffx/ffx.stamp
    fx build ffx  149.40s user 6.37s system 134% cpu 1:56.10 total
    
    Change-Id: Ia0f1b1544280e995ee58384ff057f37ce1105688
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/581512
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit c11843172db802acf2c1b0173279ad220b7c1aa1
Author: Matt Boetger <boetger@google.com>
Date:   Wed Sep 15 19:28:06 2021 +0000

    [ffx] Create args_sources to prevent recompile of all plugins
    
    Using args_sources prevents a full rebuild of ffx and all plugins. While
    the performance gain is not huge on multi-core systems, the build
    definitely takes up less resources.
    
    Tested:
    
    A change in `ffx target flash` plugin before:
    
    ╰─❯ time fx build ffx
    ninja: Entering directory `/Users/boetger/fuchsia/out/default'
    [122/122] STAMP obj/src/developer/ffx/ffx.stamp
    fx build ffx  336.31s user 24.59s system 259% cpu 2:18.84 total
    
    A change in `ffx target flash` plugin after:
    
    ╰─❯ time fx build ffx
    ninja: Entering directory `/Users/boetger/fuchsia/out/default'
    [29/29] STAMP obj/src/developer/ffx/ffx.stamp
    fx build ffx  159.49s user 6.27s system 134% cpu 2:02.98 total
    
    Change-Id: I2140c5053e68f48e1c21332bddb3f2cc9b4bcfaa
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/581507
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>

commit 30b42d7adebec34dda429999e524c6533c660fee
Author: Matt Boetger <boetger@google.com>
Date:   Wed Sep 1 20:56:22 2021 +0000

    [ffx] connect FMS to flashing
    
    Currently SDK flashing only works with in-tree SDKs.
    
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: I0c663553d51a3ceb48787e1ccdf735706b762141
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/546621
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Renato Mangini Dias <mangini@google.com>

commit be826d6e799a54f3ee6a08000bd43ea4775ce552
Author: Matt Boetger <boetger@google.com>
Date:   Wed Aug 25 18:40:57 2021 +0000

    [ffx] Make device_id_proxy optional
    
    The results from the try_join! were all mis-named and out of order.  I
    renamed the results in the proper order and everything is working
    according to the unit tests.
    
    From thread: https://chat.google.com/room/AAAA6CXS088/CbPqKnKwXF4
    
    Change-Id: I9b84783a6c33412b9cd49375ab4d7c36c7bd6b48
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/572560
    Reviewed-by: Francois Rousseau <frousseau@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 3da36f38c74635cf114d5b7678da10083984698c
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 20 23:50:27 2021 +0000

    [sdk] Create Product bundle metadata enum
    
    It can be an int, string, or bool.
    
    Change-Id: Ie021e1dff1a1ba75702c5976de591468e60e34f6
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/572027
    Reviewed-by: Misha Gridnev <gridman@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 43d0478ec0e61bcb4fd22aff070d4bd48619569f
Author: Matt Boetger <boetger@google.com>
Date:   Thu Aug 19 22:40:39 2021 +0000

    [fms] Update FMS to V3 of the Flash manifest
    
    Change-Id: Idc474febb699eb86ea71a08abb56e8c0c2511c33
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/546545
    Commit-Queue: Omer Lev-ran <omerlevran@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Misha Gridnev <gridman@google.com>
    Reviewed-by: Dave Schuyler <dschuyler@google.com>

commit abe0060f108dfbb8dda51a5a18669d6bad90a36c
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 3 17:42:30 2021 +0000

    [ffx] Fix TAR archive flashing.
    
    Change-Id: Ied9b20959277d26d79076a19894b1796db45308e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/562841
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Andrew Davies <awdavies@google.com>

commit d15d36cd0420548f357556d1dd92f79ffb4596ef
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 28 17:54:39 2021 +0000

    [ffx] Fix reboot issue with NUC flashing.
    
    It's impossible to know if the target will need USB or UDP transport
    before we reboot into fastboot.
    
    Fixed: 79631
    Change-Id: Ic35838c8de68fc65054d25c2628c62f32068aab7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/559458
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Vincent Belliard <vbelliard@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 1b17faeb9e156aabdb0df941a2d3f1e26b2aa113
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 25 00:11:15 2021 +0000

    [ffx] Fix Flashing Reboot issues
    
    Change-Id: Iddcc5567f2d23ea3a3835809e1eb2002794584c6
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/547920
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 81db50165820130b427a11461c0ec81026844332
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jun 23 23:10:36 2021 +0000

    [ffx] On reboot, check target state after timeout
    
    If the target reboots, but we for some reason miss the event from the
    daemon, just check the target state after the timeout and return OK if
    it's in fastboot.
    
    Change-Id: I7d4cd3e6be11a56bafa0d1b62e0045d8ba051950
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/546462
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit d2300d92d75b9f9c5209ba461d6399009b232b5c
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jun 22 00:54:12 2021 +0000

    [ffx] Update fastboot check interval time
    
    Since fastboot over network is only broadcast every 10 secs, fastboot
    over network targets will be timed out before rediscovered.  Bumping
    this value up should fix it.
    
    Change-Id: Ia89f89c930ef82cfc060826bb1c0fcfcaa0b3831
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/545953
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 7d082ac79b7c3e46538d66d13bc57affa615dae1
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jun 22 00:33:32 2021 +0000

    [ffx] fastboot udp impl
    
    Implements UDP transport in AsyncWrite/AsyncRead interface according to
    this spec:
    https://android.googlesource.com/platform/system/core/+/refs/heads/master/fastboot/
    
    Fixed: 78713, 78714
    
    Change-Id: I738dd7a8afe12005ee50039584bab28be8bd6b37
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/534881
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 62d26ffd7e1177966dc27f524499907ff3b91b39
Author: Matt Boetger <boetger@google.com>
Date:   Sat Jun 19 01:10:05 2021 +0000

    [ffx] fastboot discovery via mdns
    
    Fixed: 77008
    
    Change-Id: If13856943526de61527721d27db3879092a132ef
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/542251
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 16a70e8e1c28b9164333677a2add284899183b41
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 18 23:28:48 2021 +0000

    [ffx] Remove the converts in Target
    
    Converting from TargetAddrEntry to TargetAddr was leaking information
    that was stored on the TargetAddrEntry - I removed most cases of it, I
    believe the most problematic case as in the addrs_merge method.
    
    This is also preparing for fastboot TargetAddrEntry
    
    Fixed: 76325
    
    Change-Id: Iac3deb8a0e22c6b3a723187c21baae37a9b53db3
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/544923
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit f4b81b7f1375e15bd2ea41f70473bf37aab8bdf6
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 18 19:08:43 2021 +0000

    [ffx] Add " (default)" to error messages
    
    Change-Id: Ide5c3cbe693d990fcbbf4e1586099f55ef2aa9d4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/544170
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>

commit 423706abdc760cd76e0e1c6bc750ce94a3f145eb
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jun 16 22:31:26 2021 +0000

    [ffx] Fix Zedboot command and control
    
    fxr/531922 removed a TODO and workaround with actually fixing the TODO
    
    Fixed: 78874
    Change-Id: I0949ca03ace8782dbd2f78d82755a3b3d78a0817
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/543969
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit ed464a9dfab8f2a0b79f0b73e5b212a681bd17ee
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 10 22:22:58 2021 +0000

    [ffx] Adjust Fastboot error messaging
    
    Fixed: 78020
    Change-Id: I078fd267fc35d54fc6884256beb95c777a2e61f9
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/541063
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>

commit 8b26d84a8220e44ab5fabe6c531a8481720268c7
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 10 21:48:20 2021 +0000

    [ffx] "Fix" `ffx target remove
    
    This provides a workaround for a race condition in the daemon when `ffx
    target remove ...` is called.
    
    Fixed: 77892
    Change-Id: I1204dc16b8800918a68db33ad0cfba8f9bb133ed
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/541145
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>

commit 58ce75d8799669a7b21da59e2a5f5784a45d10f4
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 10 21:22:35 2021 +0000

    [ffx] If no targets are found, report "No devices found."
    
    Fixed: 78021
    Change-Id: Ie33b06affd5f1c5387990c9b282a32c19f0eaa0a
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/541345
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    API-Review: Dave Schuyler <dschuyler@google.com>

commit 70994f4b95a5f9d0c15c95e3fb93d131c1273a13
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 4 19:56:53 2021 +0000

    [ffx] add skeleton code for fastboot network transport
    
    Change-Id: I8d709faf5a80260c8f3d9461c1456925b7c7a7b8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/533568
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit b35ff5c3f6ec315478df8d0c776af4c59e27e7a3
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 20 23:52:53 2021 +0000

    [ffx] Add tarball support for flashing
    
    Fixed: 77106
    Change-Id: Iddf5c99bcd89098eaeeef962782c012cbabf6a4c
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/532401
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: James Tucker <raggi@google.com>

commit 162975345b1c0ab06c97cbb682c2e82488a333ae
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 20 19:03:01 2021 +0000

    [ffx] Add "--no-bootloader-reboot" switch for `ffx target flash`
    
    Fixed: 77194
    Change-Id: I2bd9da0fbb542e996705c46667dae551920b2c24
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/532864
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Amit Uttamchandani <amituttam@google.com>

commit f93c900ed7bf1bf887c25ceac76fdf5d00e26956
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 19 20:50:32 2021 +0000

    [fx] Update fx-flash script to use the new ssh key flag
    
    Change-Id: Ic21b805db44c46f492373e1f233dbd1e4b322411
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/515781
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Reviewed-by: Renato Mangini Dias <mangini@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 2421132f19fecf78bf36fa50a209bb9209d511bc
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 13 18:25:51 2021 +0000

    [ffx] zedboot reboot command
    
    Now `ffx target reboot` will work if the device is in Zedboot. `ffx
    target flash` will also attempt to reboot a Zedboot device back into
    Fastboot before flashing.
    
    MULTIPLY: ffx_daemon_lib_test
    
    Fixed:7546
    
    Change-Id: Iac2a37cb34d42eba2862f9143dbdef7a2358bd8a
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/526836
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    API-Review: James Tucker <raggi@google.com>

commit c3a5428734db613ada818c61b70e346a580df0b4
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 13 01:09:01 2021 +0000

    [ffx] Zedboot Discovery
    
    MULTIPLY: ffx_daemon_lib_test
    
    Bug:75463
    
    Change-Id: I2adaac2526d48fb86a55b036191d1a13c67d7ba1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/526227
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    API-Review: James Tucker <raggi@google.com>

commit 722a95920d392e7eb4e691b8a865194716f7ff2b
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 6 19:17:51 2021 +0000

    [ffx] Reboot to fastboot when flashing
    
    This will reboot a device into fastboot when running `ffx target flash`
    if the device is not in fastboot state.
    
    Fixed: 69285,75969
    Change-Id: Ia98c0087021b4a8518bba8e1a4ce1c6b4d873729
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/523148
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit ac95fcc42fabe5d80b37c8d51085efd4c1fb2a93
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 5 01:28:17 2021 +0000

    [ffx][starnix] Return exit code directly from plugin
    
    Change-Id: I88fa9d17a02a0ac7e5eaf7750168cfb39cfa9166
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/525332
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Adam Barth <abarth@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit ad194e28e5ceb0578b19e4c65dc76c59ced85ed5
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 5 00:24:33 2021 +0000

    [ffx] Allow plugins to return a custom exit code via Result<i32>
    
    This allows plugins to return a Result<i32> to specify a custom exit
    code without assuming an error.
    
    Change-Id: I8c676fe521d738fc12d1e2eb5514ca0f7e3c094c
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/513500
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit f68367c89dd5879beafc8bc467063183bfa93807
Author: Matt Boetger <boetger@google.com>
Date:   Mon May 3 22:40:01 2021 +0000

    [ffx] target list names target not found
    
    This also splits the error code functionality from ffx_bail/ffx_error to
    ffx_bail_code/ffx_error_code.  Having the error code at the end of the
    parameter list causes problems with the macros that end in $($arg:tt) -
    so the error code needs to move to the front of the list.  Also, it
    would be nice to allow expressions for error codes.  Both of these
    changes made the new macros nessecary.
    
    Fixed: 75829
    
    Change-Id: Idd3b3f39ac77fe01da1e757174cc7ab5399f9038
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/523985
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 93cceed50c9d8ad3b379f1a2fd5282d17b2643ca
Author: Matt Boetger <boetger@google.com>
Date:   Fri Apr 30 20:54:45 2021 +0000

    [ffx] Do not limit flashing by "json" extension
    
    Engineering builds use ".manifest"
    
    Change-Id: I488af678605a5f042fd2bf4425b2737d5ff66d7b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/523154
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 56812f6030f072cc84bdf2873307b93ed6b98b28
Author: Matt Boetger <boetger@google.com>
Date:   Fri Apr 30 01:08:23 2021 +0000

    [ffx] Support flashing from a zip file.
    
    Fixed: 75688
    Change-Id: Ica3c8b96a7847e5e4d91ca845842733a426b75a7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/522661
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 545a693eabe7c282de7e1560a3ee64f24f6988d1
Author: Matt Boetger <boetger@google.com>
Date:   Fri Apr 30 01:01:00 2021 +0000

    [images][ffx] Move to v3 for flash.json
    
    Version 3 is a more explicit object instead of using array.
    
    Change-Id: I0afe7378e389bfba1115e1a32782029195ddf6e1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/521861
    Reviewed-by: Omer Lev-ran <omerlevran@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>

commit 6792153ea9edb4f33edaf238eb5b2d28b0138186
Author: Matt Boetger <boetger@google.com>
Date:   Wed Apr 28 22:24:22 2021 +0000

    [ffx] Create Target FIDL
    
    This hides the reboot functionality behind the target connection state
    for better error messaging.
    
    MULTIPLY: ffx_daemon_lib_test
    Fixed: 74867, 74186
    
    Change-Id: I271166653b562df31e66ea563a00976712f4cc84
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/517600
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    API-Review: James Tucker <raggi@google.com>

commit f1bbd605f601b4799829dc4b5b3560c0c21a4238
Author: Matt Boetger <boetger@google.com>
Date:   Wed Apr 28 19:07:10 2021 +0000

    [ffx] Only get one remote control connection
    
    This prevents plugins with multiple mapped proxies from getting multiple
    remote control connections.
    
    Change-Id: I468a0ea8d8fdfc13404f4bfd8a00af0d3992c2d4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/520063
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 81c0b099b8a312eb72189d3d959dc8eac452195d
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 27 19:29:15 2021 +0000

    [ffx] Create v3 flash manifest
    
    V3 contains an explicit structure.
    
    Fixed: 74889
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: I4eea3ad24db3b3a6273a3c49c5a02520ceabb5a4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/520102
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Casey Dahlin <sadmac@google.com>

commit 184f7cd61cf843acc04634669711c26ad0d243d6
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 27 18:13:50 2021 +0000

    [ffx] Implement default ValueStrategy
    
    Change-Id: Ie898e760d96d64d47f06206c38af07ad7f7c2c69
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/521121
    Reviewed-by: Casey Dahlin <sadmac@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 7781a92d10def78b9aec754a33825f27fa7095f4
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 27 18:12:59 2021 +0000

    [ffx] `ffx target flash` prints total time
    
    Fixed: 75439
    Change-Id: I4a34e1da297bdeeac390737de07cd361e55765e2
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/521095
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit a488159eba2706f84f228756218d7f893babfa24
Author: Matt Boetger <boetger@google.com>
Date:   Fri Apr 23 03:01:15 2021 +0000

    [ffx] remove unnecessary ffx_config::Value
    
    Change-Id: I841f29c1cf0da240db9489953652b0c1380ef919
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/519880
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Fuchsia-Auto-Submit: Andrew Davies <awdavies@google.com>

commit 65f6f5a32efc233ebb800eeda8dba0cfe3468a09
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 22 19:18:01 2021 +0000

    [ffx] Fix float conversion from config
    
    Fixed: 75217
    Change-Id: Ida7fc4eae02508dfa1b0eea499a14cbdf7049128
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/519663
    Fuchsia-Auto-Submit: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andy Weiss <dragonbear@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit 7ac014d42669730c40cd4e32548b3eb6faa01589
Author: Matt Boetger <boetger@google.com>
Date:   Wed Apr 21 00:22:15 2021 +0000

    [ffx] Add more explicit error messaging.
    
    This add the matcher used to the error messages for the NoTargetFound
    error messages.  Also, if the matcher is empty, it assumes no targets
    are connected.
    
    Fixed: 74900
    
    Change-Id: I1d649ab128c57325dc1d95e9831a344cb660d9bb
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/518902
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 7720eb739666b4c123742ba0c4cb8a3fe964fa0a
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 20 19:03:18 2021 +0000

    [ffx] Wrap plugin injections in single Injection
    
    By creating a single Injector trait, the ffx plugin signature is
    simplified.
    
    This appears to help with memory usage as well as compile
    time/parallelism while compiling:
    
    HEAD: fx build ffx  495.12s user 170.13s system 384% cpu 2:52.93 total
    CL: fx build ffx  362.33s user 166.46s system 1134% cpu 46.609 total
    
    Bug: 74452
    MULTIPLY: ffx_core_impl_lib_test
    Change-Id: I767cf94166f42eaac2ea0a5e1f6e4856c9582ca9
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/518460
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>

commit 3a88bb1e2bc60ec998c3ad9430b9dc28b15aaec9
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 20 02:42:20 2021 +0000

    [ffx] Add conditional partitions to flash manifest
    
    This will allow conditional partitions based on variable values.  For
    example, partitions defined like:
    
    ["partition_name", "path", "var_name", "var_value"]
    
    Will only flash to the device if the fastboot variable "var_name"
    matches the given "var_value".
    
    Fixed: 64549
    MUTLIPLY: ffx_flash_lib_test
    Change-Id: Ie36702c0a8083545293847078d6606f38267e457
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/517685
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 0aa2206b044bff841e0ee770100f3b32903f7500
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 20 01:24:39 2021 +0000

    [images][ffx] Update flash.json to version 2
    
    Version 2 includes the board name to allow for board verification before
    flashing.
    
    Fixed: 74508
    
    Change-Id: Ie731c2aa1713d1d12d7ed403089bf66bb918bfbb
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/516820
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>

commit dd091f7201f8df2488153f227984ef56c48a8656
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 19 23:37:22 2021 +0000

    [ffx] Verify hardware before flashing
    
    Bug: 74508
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: I1e4996ade13c6f03e71cb9a21b414d1fda71eccc
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/516529
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Casey Dahlin <sadmac@google.com>
    API-Review: James Tucker <raggi@google.com>

commit 6901dd1fbc3e6d138f6bf6f58bea5485cbc4af34
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 19 22:16:34 2021 +0000

    [ffx] Move V1 flash manifest code.
    
    This will make it easier to add a v2 later on.
    
    Bug: 74508
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: Iab2438a7d8085d618a9b6c67b748fb8f7e467f61
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/516173
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 682795d53242c761741ed3049a727a332d304e97
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 19 19:55:18 2021 +0000

    [ffx] Add `ssh-key` flag to `ffx target flash`
    
    The ssh param is a simplified version of the OEM stage param
    specifically for the `add-staged-bootloader-file ssh.authorized_keys`
    OEM command. If the key is not supplied, it will now check the config
    for the ssh public key to ensure ffx can connect after flashing.
    
    It will also look for a default "fuchsia" product if no product is
    supplied via the CLI and there are multiple products found.
    
    MULTIPLY: ffx_flash_lib_test
    Fixed: 74314, 74307, 74313
    
    Change-Id: I7cc74f182e27937f49ecf223de0c3928e32996a4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/515610
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 77bc434df26bd94133c4da2993efe95ea1744fef
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 15 22:15:57 2021 +0000

    [ffx] add a timeout for get_hash
    
    Change-Id: I630c4473deb69afbd73bca0f44304cb04e5de9ee
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/507381
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 6b415be888204c46789944dc39b4ee8a8e4389dc
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 15 22:07:55 2021 +0000

    [ffx] Make sure the USB interface is cleared
    
    This will make sure the USB interface is available again to use if the
    user Ctrl+C during the middle of a flash.
    
    Change-Id: I0762b2789b30d69116cd70d9ae2710d5549b93a7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/515929
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 82bc6b328622bc0c58bcfbb416d34cc9c678a3e3
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 13 20:12:18 2021 +0000

    [ffx] Change setup test proxy closure to FnMut
    
    You will still need to wrap variables in Arc<Mutex<_>> to interact with
    a clone in the closure.  And as async closures are not yet supported, it
    will need to be std::sync::Mutex.
    
    Fixed: 70310
    
    Change-Id: Ie228d5e31c0d68415733c5710b9ad0ac3efe3b10
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/513846
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 4458979bad13bd6dd3cabbd75280ce6dc91f15df
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 12 21:12:26 2021 +0000

    [ffx] Add a warning when rebooting to recovery
    
    Fixed: 74259
    Change-Id: Ibeecaebf6fcf7fb51afbb101a5df67bcbeca9b0b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/513984
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Amit Uttamchandani <amituttam@google.com>

commit 58baa3aef7eec1f5605fe8c0e4d46ce8601ebd70
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 6 18:17:28 2021 +0000

    [ffx] Fill in state for `ffx target list`
    
    Change-Id: I93a1a914cee8503f5192aedba740fb27f71313b3
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/510788
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    API-Review: James Tucker <raggi@google.com>

commit e6b6363427d9a172409746631782c5d7d0b3d847
Author: Matt Boetger <boetger@google.com>
Date:   Sat Apr 3 00:02:33 2021 +0000

    [ffx] Generate flash.json for the archive
    
    Just like flash.sh needs a special target for the archive, so does the
    fastboot_manifest for ffx.
    
    Change-Id: I92bbe4a7ced517a9e37fd76d21b78d88de2818b2
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/508202
    Reviewed-by: Aaron Wood <aaronwood@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit be90ed225b2a69f24ffed1ad77bf3e9be3728e3f
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 1 18:04:12 2021 +0000

    [ffx] daemon should return DaemonError for GetFastboot
    
    To make sure we can use the same Daemon specific errors, GetFastboot
    should throw DaemonErrors.
    
    Fixed: 72914
    Change-Id: If577af13f6a2b8921933d465500288672a8a7ca8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/506458
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Casey Dahlin <sadmac@google.com>

commit 9908e150b3a95dd2b5e70dea4593ca1beae35057
Author: Matt Boetger <boetger@google.com>
Date:   Mon Mar 29 23:11:10 2021 +0000

    [ffx] Make sure to give the full path to the Daemon for flashing
    
    This allows the manifest path to be passed in as a relative path.
    
    Fixed: 73264
    
    Multiple: ffx_flash_lib_test
    
    Change-Id: Ic8e11f09a154f2cf9f90703661b9e3952706c2ed
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/508072
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Omer Lev-ran <omerlevran@google.com>

commit 807bd36a8e7f4f177d4d330a56d18b89ffadf2f6
Author: Matt Boetger <boetger@google.com>
Date:   Thu Mar 18 23:05:52 2021 +0000

    [ffx] Assume ClientChannelClosed is a success for `ffx target off`
    
    Bug: 72536
    Change-Id: I91e625755060a32097ce85792f8398c8c6518031
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/503541
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 81dae588d8c299786746ffcb18bcb65c3dfd8730
Author: Matt Boetger <boetger@google.com>
Date:   Thu Mar 18 02:53:54 2021 +0000

    [ffx] Fix the Mutex in main to be async
    
    Change-Id: I9d9076b558e25c04b4b4c77b2fcc19984ed610fa
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/503839
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 0c629f7412ec00fea06297fef2f5a43539b0817c
Author: Matt Boetger <boetger@google.com>
Date:   Wed Mar 17 22:30:04 2021 +0000

    [ffx] Clean up differences between mapped_proxy and known_proxy
    
    Change-Id: I558839ed089bf74c0022a3355f155ac41f8d9cda
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/500968
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 6799a3ec4adc77768db64c3299f0f71f7b892a06
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 16 22:25:37 2021 +0000

    [ffx] logging code drop the turbofish for config calls
    
    Adding usize as possible value from config.
    
    Change-Id: I090814cb2cd12f4784d480a6ec96f325c91254ea
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/502721
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 4d50734febf1774733613472c1d4d0639fd24147
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 16 21:54:32 2021 +0000

    [ffx] Add nodename and ssh address to `ffx target show`
    
    Multiply: ffx_target_show_lib_test
    Bug: 71235
    
    Change-Id: I9d70f678944a2756ebf3bde7d6692aebff856f52
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/502219
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Dave Schuyler <dschuyler@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit c60a7f0bc80c066325b869936bdcacac58bf431f
Author: Matt Boetger <boetger@google.com>
Date:   Fri Mar 12 17:26:37 2021 +0000

    [ffx] Allow Result and Option Proxy params in ffx_plugin
    
    Note: now every proxy in the parameter list creates its own
    RemoteControlProxy (thus making several calls to the Daemon to get the
    RemoteControlProxy).  This makes the ffx_plugin code simplier at the
    cost of a little bit of performance (all the connections still happen in
    parallel).
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: I3f5478b7f29ce9da6954a78b2a018aadcea644a1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/500362
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 53f6ba395be1c02929ea4652157cbe7f7844e8da
Author: Matt Boetger <boetger@google.com>
Date:   Wed Mar 3 20:44:05 2021 +0000

    [ffx] Flash.json now generated with relative paths
    
    Bug: 71220
    Change-Id: I413ccc8fcb51e229d13dbbacfcd1a45f8a012ced
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/493659
    Reviewed-by: Dave Smith <smithdave@google.com>
    Reviewed-by: Renato Mangini Dias <mangini@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 6757e92967dd6060405955d38a23a2a1ffafc666
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 2 22:06:41 2021 +0000

    [ffx] Use an error code of 2 to indicate No value found.
    
    Bug: 70930
    
    Change-Id: Icba378daa4a284ae3404f056fb3fee31c8964a6f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/492898
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 5e8f8e6bd87961006b9eaf0687f51b0a78653c4e
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 2 00:46:29 2021 +0000

    [ffx] `ffx target flash` works with relative paths
    
    MULTIPLY: ffx_flash_lib_test
    Bug: 71220
    Change-Id: I671e8a9f7e4d1c4aaa5ffa4eb3f6293ae8d6bc6f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/493678
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 4bfc0f02683261df394b0f87ee5cd7a528d9877c
Author: Matt Boetger <boetger@google.com>
Date:   Sat Feb 27 00:55:21 2021 +0000

    [ffx] harden fastboot code against multithreaded issues
    
    Change-Id: I363f67ad1556d99aff8ca5026de8128384086989
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/492722
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit e013c5fc0aa9a5df5c51af0f15b555b63cc19679
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 26 23:47:18 2021 +0000

    [ffx] Add flashing rate and minimum timeout to config
    
    Change-Id: I04e635d4da5abc6a234807f956b3cfdfec51e6ce
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/490766
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit dd7b7170d9c36d072c8b8491e386bb6e9b3b5f79
Author: Matt Boetger <boetger@google.com>
Date:   Thu Feb 25 17:51:56 2021 +0000

    [ffx] Remove brittle tests in ffx_plugin impl
    
    These tests are extremely brittle and almost impossible to gather any
    useful information from failures.  I have remove these tests and
    replaced as much as I could for now with less brittle tests. The
    ultimate test for this code is if ffx actually compiles.
    
    Change-Id: Ibaf57dd67aaa7111cb1a0952e7759db1322ff069
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/489298
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 4de25f2c84ead409bb174bec611f347635420952
Author: Matt Boetger <boetger@google.com>
Date:   Thu Feb 25 17:47:16 2021 +0000

    [ffx] UX polish for ffx
    
    Bug: 70468
    Change-Id: I0117cd4cfa76af058d5f6baa9c39bd723534dc64
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/488410
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 16d0af92c7169323b038d55a7fe9f41d89ba4b9b
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 19 19:44:30 2021 +0000

    [ffx] clean up core impl for ffx_plugin
    
    This just splits up the one large function into several smaller
    functions.  I kept the tests the same for now to make sure everything
    still passes.  I did change one test that tests the daemon, fastboot
    ordering.  It shouldn't really matter the order the factory functions
    are called.
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: I976dbd07da5b761d1039de54837c88a86a1e877d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/488600
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 8fb24f1941348ae1affea8d0e7ff7cf0821ce129
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 19 01:41:31 2021 +0000

    [ffx] Remove underscores in ffx_plugin generated code
    
    The compiler doesn't complain about unused variables in generated code.
    
    This is the first of a few cleanup CLs.
    
    MULTIPLY: ffx_core_impl_lib_test
    Change-Id: I0a6c04f89fbefaeb951f6159103d5a6635f52fa8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/487893
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 4f83b30b35f893584e2cbbc6fa4214806c0a2602
Author: Matt Boetger <boetger@google.com>
Date:   Thu Feb 18 02:58:45 2021 +0000

    [ffx][usb_bulk] Implement AsyncWrite and AsyncRead in the usb_bulk library
    
    Bug: 69059
    
    MULTIPLY: ffx_daemon_lib_test, ffx_flash_lib_test
    
    Change-Id: I34f5fa4ac1c6c075253d3c2e568c63838c8fdb4d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/485081
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    API-Review: James Tucker <raggi@google.com>
    Fuchsia-Auto-Submit: James Tucker <raggi@google.com>
    Commit-Queue: Auto-Submit <auto-submit@fuchsia-infra.iam.gserviceaccount.com>

commit e4d9aa766e40819fb173f524213042e20cd7e47d
Author: Matt Boetger <boetger@google.com>
Date:   Tue Feb 16 20:05:29 2021 +0000

    [ffx] Remove output type
    
    Just default to JSON output
    
    Bug: 68931
    
    Change-Id: Ic06838d363e3f44118f61dd7d457ba35041a3079
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/480147
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 47a26539712b3c6dbe00c90268d177e38439c017
Author: Matt Boetger <boetger@google.com>
Date:   Sat Feb 13 00:17:32 2021 +0000

    [ffx] Assume reboot successful if there's a ClientChannelClosed error
    
    Bug: 11044
    Change-Id: I029082edb0507d226e01ef03c2786303f11b4589
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/484760
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 7caf30e2ec713849ba654c25ab553f31a423d689
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 12 22:19:34 2021 +0000

    [fconfig] Use the default JSON output of `ffx config get`
    
    Change-Id: I4796ec19a306f9a580f4ce09326d828956600577
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/480146
    Reviewed-by: Clayton Wilkinson <wilkinsonclay@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 66f0713afbfdfd0ed13286071f73bbaa0fccb53f
Author: Matt Boetger <boetger@google.com>
Date:   Mon Feb 8 21:43:21 2021 +0000

    [ffx] Set the default output type to JSON
    
    The option to change this will be removed after fconfig is migrated to
    use the JSON output.
    
    Change-Id: Iea950464b8311ac5d2ef2b54332d16aede92b709
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/480077
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit b244f6dfa4e157deb02734a4ed35cefe85429282
Author: Matt Boetger <boetger@google.com>
Date:   Mon Feb 8 21:12:18 2021 +0000

    [ffx] Add better error messaging when connecting to targets
    
    When you attempt to run `ffx target flash` against a device not in
    Fastboot, there needs to be better error messaging.
    
    Same with running RCS commands against a Fastboot device.
    
    Bug: 69058
    
    MULTIPLY: ffx_daemon_lib_test
    Change-Id: Ic94957ca195331010d328fd861a701ed788a3737
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/482461
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit afb8becc50498376b5e439bf6c6d478be3abcb7a
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 5 20:00:36 2021 +0000

    [ffx] Allow custom error codes
    
    Change-Id: Ife7fb905e906a1483570f757d11ff3efa5ae527e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/481918
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 9de5ba1720d22317a116ddd52564fd092d331c2b
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 5 00:33:29 2021 +0000

    [ffx] Add JSON format to `ffx target list`
    
    Bug: 68072
    
    Change-Id: Ifccaf3ab32242038bbcc6ae1aee95f0f62769d8e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/474116
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 7d30d3321d0b9d102814282fc6726a47c4857565
Author: Matt Boetger <boetger@google.com>
Date:   Wed Feb 3 23:43:30 2021 +0000

    [fconfig] Explicitly use the "human readable" output.
    
    The default output for `ffx config` is going to change to JSON. This
    flag will need to be used until fconfig code can be changed to use the
    JSON output.
    
    Change-Id: Ic707ea51bc947e7eacdb802287a84470985a2642
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/480052
    Reviewed-by: Clayton Wilkinson <wilkinsonclay@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 627d11fde9faa9b0c6cab9656a506dc13c959f0d
Author: Matt Boetger <boetger@google.com>
Date:   Wed Feb 3 22:14:20 2021 +0000

    [ffx] `ffx config set` can now accept JSON
    
    Bug: 68350
    
    Change-Id: Ib155c93a1816468740f9bde5de7048ac94a43aad
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/480051
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 05a8c7266b71b6b8541974c93ebdccf699b3e2f3
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jan 21 19:22:56 2021 +0000

    [ffx] Add `ffx daemon log` to dump the daemon log file.
    
    Change-Id: I725786f41cd3b34bb37d526a518b758e238324ef
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/470599
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 9e7546a54a3880a8ea660dd8d5c9439b94019ab4
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jan 20 23:47:44 2021 +0000

    [ffx] Check the hash of the binary
    
    To make sure the frontend and the daemon are in sync, hash the binary,
    and check the hash against the daemon when connecting.
    
    Change-Id: Idcf4cac0fcc08418aa44250fb733894d63e1e601
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/468900
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    API-Review: James Tucker <raggi@google.com>

commit a69d5ab735dd1b111b1696c5e0a0994375995575
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jan 12 21:56:59 2021 +0000

    [ffx] Turn on logging by default
    
    Also create mappings for $RUNTIME, and $CACHE in the config system as
    well as adding MACOS equivalents to XDG_RUNTIME_HOME, XDG_CACHE_HOME,
    XDG_DATA_HOME, XDG_CONFIG_HOME
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I9b0e43dc4e0c7b0bfba5c1108de86ab5faa29d41
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/468036
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 543846bd34c8e32edd39917f5ac28a0aabd80836
Author: Matt Boetger <boetger@google.com>
Date:   Sat Jan 9 00:33:08 2021 +0000

    [ffx] Add help text to end of the ffx.
    
    This will print 'See 'ffx help <command>' for more information on a
    specific command.' at the end of any ffx help <COMMAND> invocation.
    
    BUG: fxb/63367
    
    Change-Id: I296504cc1d85c3fc8535351aa58f990c01663fda
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/463265
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 7de9ca209924aa5e8e265dc378b365ab33717100
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jan 8 22:56:24 2021 +0000

    [ffx] Replace fastboot flash.sh with ffx
    
    Change-Id: I0b3ad9031bef68f642f3214e8b6a85b53413c38f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/460021
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: David Pursell <dpursell@google.com>
    Reviewed-by: James Tucker <raggi@google.com>

commit e7913360f9e9850f13338b436de61c23a8be05a2
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jan 5 22:40:58 2021 +0000

    [ffx] Allow for oem commands to be passed by the command line
    
    This will be used to handle the fx flash use case.
    
    Change-Id: Ice7b4200abe0cff3ab660d31b445e6783cbdb83f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/458472
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 10ba48d4c966e5308c3b55f5d923b245b050e91e
Author: Matt Boetger <boetger@google.com>
Date:   Thu Dec 10 20:14:22 2020 +0000

    [ffx] fuzzy matching for target selection
    
    MULTIPLY: ffx_daemon_lib_test
    
    Change-Id: I2aec4f19519c3c34cf888d47e55431f18e9c3fef
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/459977
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit edd3b9e867a1e494adbd3b80ed1168d04a096b79
Author: Matt Boetger <boetger@google.com>
Date:   Thu Dec 10 00:44:14 2020 +0000

    [ffx] Add a fastboot connection state
    
    Change-Id: Icfe003e00ae5df9d31fec09f590da048799e2438
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/458290
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 134e683c1ec1898a71d3988b82ef2b12be541050
Author: Matt Boetger <boetger@google.com>
Date:   Fri Dec 4 23:10:52 2020 +0000

    [fuchsia-hyper] Use futures instead of std
    
    Change-Id: I667436af544d9b5570324d04eb8b221177ae2e8e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/457023
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 34cbec79918cc70f975971f34d1e194f93fa59cf
Author: Matt Boetger <boetger@google.com>
Date:   Wed Nov 25 20:06:40 2020 +0000

    [ffx] Remove copy requirement for testing methods
    
    Change-Id: Ie2e5c96f17c6ce595ae7adf3e8dc63eb6c58f058
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/455436
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 8e0567b9eba37c66e2acccb605932ff92e4c80a4
Author: Matt Boetger <boetger@google.com>
Date:   Fri Nov 20 19:08:41 2020 +0000

    [fuchsia-hyper] Move fuchsia-async to dep for both host and target
    
    lib.rs uses fuchsia-async::Task - so it's needed for both host and
    target
    
    Change-Id: Id44f8761edd0b0b4fe003bc4ac44152937e12020
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/453338
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 99acdca7d79570363d5938d92273fc5d39b6cad3
Author: Matt Boetger <boetger@google.com>
Date:   Thu Nov 19 18:30:51 2020 +0000

    [ffx] Updating README.md to point at getting started docs
    
    Change-Id: I4f463bfd680ad45bdea137550f5df3c2cbe28819
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/442619
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Nick Van der Auwermeulen <nickvander@google.com>

commit 516f428aec955d2677cc78442706cfd994ca1ebb
Author: Matt Boetger <boetger@google.com>
Date:   Thu Nov 19 17:33:10 2020 +0000

    [fuchsia-hyper] Cross compile fuchsia-hyper using async-std compat
    
    MULTIPLY: fuchsia_hyper_lib_test
    
    Change-Id: I11f2c4d58625b83c44eeee0b16c7872a3202bd3e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/451294
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 36fa43a48a597f51abe71f62d8037faac6900aaa
Author: Matt Boetger <boetger@google.com>
Date:   Fri Nov 13 00:09:45 2020 +0000

    [OSRB] Fix linking issue with core-foundation-sys
    
    Change-Id: Ic9c8f7f9505fadd30707a8eb980d0de5ee13c6b0
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/450235
    Reviewed-by: Adam Perry <adamperry@google.com>
    Testability-Review: Adam Perry <adamperry@google.com>
    Commit-Queue: Adam Perry <adamperry@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 791b6a0ac7f954fef2d5af1c8b119125a2d1b645
Author: Matt Boetger <boetger@google.com>
Date:   Thu Nov 12 03:40:05 2020 +0000

    [OSRB] Incorrect location for security-framework
    
    While moving security-framework to tiny_mirrors, the BUILD.gn wasn't
    regenerated from the first place I put - rust-mirrors.  This is needed
    to correct the issue.
    
    This was generated by running `fx update-rustc-third-party`
    
    Change-Id: Ia46b55a4dd5437bd042ea9a8006141ce4c5db76d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/449760
    Reviewed-by: Adam Perry <adamperry@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 621cc4895325879cb6661e5a26d32f02fc82a156
Author: Matt Boetger <boetger@google.com>
Date:   Wed Nov 11 22:02:00 2020 +0000

    [OSRB] Needed third_party crates for ffx
    
    Bug: 55328
    
    Change-Id: I7133c20caa0873544e7bc7fb0defe24cf7ecc839
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/402960
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Adam Perry <adamperry@google.com>
    Testability-Review: Adam Perry <adamperry@google.com>

commit f8365f7d230ba2d443f62f2c3b16cee80420125a
Author: Matt Boetger <boetger@google.com>
Date:   Sun Nov 8 23:41:39 2020 +0000

    [ffx] Help text polish
    
    FIXED: 63367
    Change-Id: I64efd7366bfd362552c28c978bf16ce76e8c3e97
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/447583
    Reviewed-by: Casey Dahlin <sadmac@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Amit Uttamchandani <amituttam@google.com>

commit 535ddb2733d26f09b2df57d79d33f4177dab56f5
Author: Matt Boetger <boetger@google.com>
Date:   Fri Nov 6 19:20:03 2020 +0000

    [ffx] generate fastboot manifest
    
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: I21f770d2e6325bcc8c241b9f491001c4b1b6dd0b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/445296
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Shai Barack <shayba@google.com>
    Testability-Review: Shai Barack <shayba@google.com>

commit 09fbccdac783a40b53571aac1118d67fd505445b
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 3 00:29:42 2020 +0000

    [ffx] fix flake
    
    FIXED: 63023
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: Ia7ea5e37631b469e99f16c23a1ba6603bdbd2823
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/446474
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit f963e2d8b0f773504e3fba0210f7210db44f460e
Author: Matt Boetger <boetger@google.com>
Date:   Tue Oct 27 22:39:35 2020 +0000

    [ffx] Add error codes to Fastboot FIDL interface
    
    MULTIPLY: ffx_daemon_lib_test
    Change-Id: I2230f34501f484072b689b55fc463d9940d3f576
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/434314
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    API-Review: James Tucker <raggi@google.com>

commit a7b9940343fe22b20ed118ceb01d8f6742ac3fd8
Author: Matt Boetger <boetger@google.com>
Date:   Tue Oct 27 18:09:15 2020 +0000

    [ffx] Removed unused commands
    
    BUGID: 62762
    Change-Id: I4054a17a98a38c586d2cc0f698448e177edc1376
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/443031
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Amit Uttamchandani <amituttam@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit cf11c7166e80540a5bf416b98c76827c469775cb
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 23 18:35:03 2020 +0000

    [ffx] Remove fastboot library - create module in daemon
    
    Change-Id: Iab40be982baa7ba0cfb6767c34b5aba416ed1761
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/435476
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 91982d0a3387350387da928b9d703002fdf6a1d8
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 16 00:38:01 2020 +0000

    [ffx] Add timeout for fastboot proxy - just like RCS
    
    Change-Id: I01ef8a3b477609c69fb23ae8839ca51710dc9934
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/434975
    Commit-Queue: Andrew Davies <awdavies@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 9cc91ebe89d63d8013be9e1bceeadc8564c5fe5f
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 7 21:35:05 2020 +0000

    [ffx] --config flag now also accepts a file path
    
    Change-Id: Iad128492de39566b276d8b537c9c09f2b4e313e9
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/435774
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit d62a989245421ec453d5056b8216818c2d111481
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 7 00:57:31 2020 +0000

    [ffx] Make sure dot notation works with config flag
    
    Change-Id: I03977347183ad45bd70aa6883b552bf59c484673
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/435734
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 1a8b43343d5c8da3f0ce8f836588307b3304958a
Author: Matt Boetger <boetger@google.com>
Date:   Wed Oct 7 00:13:28 2020 +0000

    [ffx] Generate files when setting up environment files.
    
    When ffx config env set is used, if the file does not exist, create an
    empty JSON file.
    
    BUG: 61151
    
    Change-Id: I734de307815373c42f71b47c8c0f7488e2cc5455
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/435138
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit c3e530b1986cf528d6d1e2ef32e27f2f936d60ed
Author: Matt Boetger <boetger@google.com>
Date:   Tue Oct 6 23:32:56 2020 +0000

    [ffx] Create an output type for ffx config
    
    This will allow scripts to get valid json from the output.
    
    BUG: 61153
    MULTIPLY: ffx_config_plugin_lib_test, ffx_config_plugin_args_lib_test
    
    Change-Id: Ieeafa6844e9e8126113bf0c596ea7760db81933f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/435121
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 29a92b4f078dddeaea02995c68238fda78f13896
Author: Matt Boetger <boetger@google.com>
Date:   Fri Oct 2 17:50:46 2020 +0000

    [ffx] Fastboot - add support for ssh keys, bootloader images
    
    MULTIPLY: ffx_daemon_lib_test
    
    Change-Id: I5c82973a240a6ac205eed1fa7b98919be0d06833
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/429004
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 1a235698af76f1ad78c84ec5c18825fe34420d99
Author: Matt Boetger <boetger@google.com>
Date:   Thu Oct 1 20:23:16 2020 +0000

    [ffx] Provide a way to get values from all configuration levels.
    
    Instead of just returning the first value found - this will return all
    values in all levels found.
    
    Change-Id: I6585f0d8bf2fc2031117b34ca4fe6e4abe886e0e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/430386
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 51e9e0dfcbaab02476f059aed9174937e9f07bda
Author: Matt Boetger <boetger@google.com>
Date:   Mon Sep 28 18:35:36 2020 +0000

    [ffx] fastboot daemon integration
    
    MULTIPLY: ffx_daemon_lib_test, ffx_fastboot_lib_test, ffx_flash_lib_test
    
    Change-Id: I77e09e7bbad365578695f6dfdb78dd49b2305212
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/428403
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    API-Review: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 5a1df7bf56711162386904f42a0e6360ecf62efd
Author: Matt Boetger <boetger@google.com>
Date:   Thu Sep 24 21:12:47 2020 +0000

    [usb_bulk] Implement Send for usb interface
    
    Change-Id: Ia4659754d1f623248ce09bdf7a176473b9559231
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/430390
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit c270371a1534776b992dddcb2ff706432a6886e2
Author: Matt Boetger <boetger@google.com>
Date:   Wed Sep 23 02:18:35 2020 +0000

    [ffx] Fastboot frontend integration
    
    MULTIPLY: ffx_flash_lib_test, ffx_core_impl_lib_test
    
    Change-Id: I8f5312f644d278a639d2931de9be95701bea9a31
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/424998
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    API-Review: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 9a6406d5e4f8b03f8f953fff948584837d185fa4
Author: Matt Boetger <boetger@google.com>
Date:   Tue Sep 15 23:21:15 2020 +0000

    [ffx] Lock down daemon spawning.
    
    The plugin system could call this multiple times via different threads,
    so the spawning of the daemon process should only happen once per
    thread.
    
    Change-Id: Ibcfa039cd652fb803c3e468a5adb807d223e9ac5
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/426014
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 3ff460e42609884aa9c268a8be3fff23f6d90bed
Author: Matt Boetger <boetger@google.com>
Date:   Tue Sep 15 21:55:45 2020 +0000

    [ffx] Remove need for proxy aliases
    
    It's possible to get the "Marker" and "Request" types from the proxy alone -
    so it's not necessary to do text manipulation to get these types in the
    ffx_plugin.
    
    This removes the need to create a type alias when declaring the
    ffx_plugin method.
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: I12201809eccb07ce4746d6b9aae90c73c12067b1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/427243
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 01b1666e8d4639d82e8109cf5fe66770408614c9
Author: Matt Boetger <boetger@google.com>
Date:   Mon Sep 14 21:07:52 2020 +0000

    [ffx] Dev product change for Fastboot
    
    Change-Id: I1580d1bedc4be9c3f474b390493757fe0b087816
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/427120
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 14da0874e4a13e4c4fb4a5faf401cfa319a39e21
Author: Matt Boetger <boetger@google.com>
Date:   Mon Sep 14 18:13:35 2020 +0000

    [ffx] Add vector support to frontend config command
    
    Example of output:
    
    fx ffx config get test
    test: {"vec":["$NON_EXISTENT_ENV_VAR_STOOPID","$HOME","test"]}
    
    fx ffx config get test --process sub
    test: {"vec":["/home/boetger","test"]}
    
    fx ffx config get test --process sub_and_flat
    test: {"vec":"/home/boetger"}
    
    MULTIPLY: ffx_config_lib_test, ffx_config_plugin_lib_test
    
    Change-Id: Ie2d998a7a8c076b8cc8b6d65d33bb06f6d769d96
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/425858
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 254cb1f9b8cbdd1caebec32ad6976d728149a029
Author: Matt Boetger <boetger@google.com>
Date:   Fri Sep 11 21:54:53 2020 +0000

    [ffx] Better error interface
    
    Change-Id: Ib1d03cf39ec7fcaeda65bd5029c5ee4b49affbc6
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/426356
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit e885f2c920a4466e716b043eb092bd54937f5e8a
Author: Matt Boetger <boetger@google.com>
Date:   Thu Sep 10 19:56:59 2020 +0000

    [ffx] Vector support for config
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I02f354496ad389978513456eb3ef16d1d3b61f95
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/425319
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 830d671cc8717f17ac8c3f6f0cf248f003e43c91
Author: Matt Boetger <boetger@google.com>
Date:   Tue Sep 8 19:21:33 2020 +0000

    [ffx] Create more mappers for $HOME, $CONFIG, and $DATA
    
    These are special values that can be used in configuration values to map
    to specific directories for FFX.
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I2c2454d9b9da943356479d5036898e367b820be8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/422116
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 45fab34d886535091ad1cf8e52aa3de68ade6a4a
Author: Matt Boetger <boetger@google.com>
Date:   Tue Sep 8 18:04:57 2020 +0000

    [ffx] make sure with_unit_tests is honored
    
    args.rs rarely have unit tests, so make that a separate parameter as
    well.
    
    Change-Id: I6e102994366b817430b0b81f3fd45629e9a9b6fc
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/421961
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 9671a3d6e9ea9b03cc42ef8e177e9b7b0144a8c9
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 28 20:19:51 2020 +0000

    [ffx] Ensure generated libraries don't create test libraries
    
    Trying to fix build time performance issues, this is low hanging fruit
    
    Before:
    fx build ffx  106.96s user 60.53s system 1212% cpu 13.809 total
    
    After:
    fx build ffx  94.39s user 52.62s system 1102% cpu 13.334 total
    
    Change-Id: I7ff92c0e2932d2719dfc97e0b3f2038b5164c9e9
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/422014
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 9347461d075f8bf7c720d3df766e0f745fa7fe28
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 28 19:34:56 2020 +0000

    [ffx] Use converts for ffx_config
    
    This uses rust's type system to determine return types instead of
    relying on the the macros to tell the underlying code.  Much clean
    interface.
    
    MULTIPLY: ffx_config_lib_test, ffx_daemon_lib_test
    MULTIPLY: ffx_packaging_lib_test
    MULTIPLY: ffx_config_plugin_lib_test
    
    Change-Id: Ifaef18df2c0fb5568f0883c742809654d1bf97bd
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/419658
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit c640e48134f623e8bfb2555bbe1728112dfc64d1
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 28 18:03:06 2020 +0000

    [ffx] Remove config's dependency to argh Ffx Command struct
    
    MULTIPLY: ffx_config_lib_test, ffx_config_plugin_lib_test
    Change-Id: I50c706186c193ccc932cde99955e4c9075f7f21f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/419162
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 3daf40d7643208463bf398da6980cb38cfc43706
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 28 00:57:06 2020 +0000

    [ffx] Move configs to .local/share
    
    Change-Id: I15aa8629bc6b201c415c48564e7cf0a9d92456de
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/421674
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 86dbe44e1bb27a95052882b3a1a244fae9e3f096
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 28 00:06:53 2020 +0000

    [ffx] Initial Flash manifest
    
    MULTIPLY: ffx_flash_lib_test
    
    Change-Id: Ia9def08f045d8e82d1b02bcfef23b00fb7526c6d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/420668
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 59722982b4a3b462275b2c9a22d5d5ebd76834cd
Author: Matt Boetger <boetger@google.com>
Date:   Thu Aug 27 23:58:48 2020 +0000

    [ffx] support non-async plugins
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: I9d678f030123659098b0ecdfeedaa23197cbd46f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/420751
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 6823c8b95c890acbbb42ab5fa56eca57e5d1d4d0
Author: Matt Boetger <boetger@google.com>
Date:   Wed Aug 19 00:42:31 2020 +0000

    [ffx] Automatically generate testing code for proxies in ffx_plugin
    
    MULTIPLY: ffx_core_impl_lib_test, ffx_knock_lib_test
    MULTIPLY: ffx_component_run_lib_test, ffx_select_lib_test
    MULTIPLY: ffx_echo_lib_test, ffx_daemon_stop
    MULTIPLY: ffx_list_lib_test, ffx_off_lib_test, ffx_reboot_lib_test
    
    Change-Id: Icf35182d62ea0cf9549bc4e37b3e719d5acfe747
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414012
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit cf90b24d850a36ba6bb9b67444253c31792130c7
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 18 23:05:02 2020 +0000

    [ffx] Print help if no subcommands are given at top level.
    
    BUG: 58444
    
    Change-Id: I9991b588b069133ab739ba2c0ef0f7d95e2ccf79
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/417889
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit ee06793210b87b782e44ab17afaba9b277e76bc0
Author: Matt Boetger <boetger@google.com>
Date:   Mon Aug 17 18:37:25 2020 +0000

    [ffx] Move daemon constants to config
    
    MULTIPLY: ffx_daemon_lib_test
    
    Change-Id: I15a104ce214be6d7dce5e022dd152da29f502dcd
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414550
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 42cbffb6ae688bcc8bc1118d5fab0899c6202fdf
Author: Matt Boetger <boetger@google.com>
Date:   Mon Aug 10 22:00:39 2020 +0000

    [ffx] First pass as help text
    
    Top level subcommands and descriptions
    
    Change-Id: I962f932d3b069111df8e93616c579ad4b0981915
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414379
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Theodore Dubois <tbodt@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 36f7bd4c95036be9850ffa803b18509dd2332851
Author: Matt Boetger <boetger@google.com>
Date:   Mon Aug 10 21:03:55 2020 +0000

    [ffx] automatically generate user configuration file
    
    Checks for the existence of configuration files when trying to set
    configuraton values.
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I2ff25d8fd9072d8063e0d46f889b0aca87cb5576
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414389
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit a524b9ff6492e2e12e8f411fb0c5e1919669a493
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 7 05:40:36 2020 +0000

    [ffx] Decouple component run from remote_proxy
    
    Change-Id: I4e1f9f5265c6c250a7607acaba6c5b1d3dd63c03
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414126
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 9fb86ca49676bbe2cc6bb2bbe0ccaaac1fdd3843
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 7 04:16:00 2020 +0000

    [ffx] Allow plugins to be gated by experiment flags.
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: Ie26b4dc238c18cc6fd05451e96238866f59a4bad
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/413449
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit e0a7fd8730abbdd5407ddb403a2f68a69ef9d7d8
Author: Matt Boetger <boetger@google.com>
Date:   Fri Aug 7 02:07:42 2020 +0000

    [ffx] integrate config with plugins
    
    MULTIPLY: ffx_config_lib_test
    MULTIPLY: ffx_daemon_lib_test
    MULTIPLY: ffx_packaging_lib_test
    MULTIPLY: ffx_bin_test
    
    Change-Id: Ic3d82fe4dd59761af4c98a5b0ef3c369077ed9c3
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/413495
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 100df6b92ca5558fcfae59b18acfd51250d236e2
Author: Matt Boetger <boetger@google.com>
Date:   Thu Aug 6 20:04:17 2020 +0000

    [ffx] Add documentation for plugins that use proxies.
    
    Change-Id: I0b9aa377631f4b3ec004fb12b37a575c26399aeb
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/407623
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit a1ac87c2f7da1f998dbc431dff6b8e464addaa01
Author: Matthew Boetger <boetger@google.com>
Date:   Thu Aug 6 04:25:21 2020 +0000

    Reland "[ffx] remove ffx_plugin_suite - just use ffx_plugin"
    
    This reverts commit 8abfa37ba637619129f2554d3513dd1b7baad0f9.
    
    Reason for revert: Fix forward
    
    Original change's description:
    > Revert "[ffx] remove ffx_plugin_suite - just use ffx_plugin"
    >
    > This reverts commit b51c52307878dbfec0baef653d9ef088dc5d6715.
    >
    > Reason for revert: python breaks users using python3
    >
    > Original change's description:
    > > [ffx] remove ffx_plugin_suite - just use ffx_plugin
    > >
    > > This allows for subcommands that are an Option - so if no subcommand is
    > > given, plugin code can execute on the top level.
    > >
    > > MULTIPLY: ffx_bin_test
    > > MULTIPLY: ffx_lib_test
    > > MULTIPLY: ffx_target_lib_test
    > > MULTIPLY: ffx_daemon_plugin_lib_test
    > > MULTIPLY: ffx_component_lib_test
    > >
    > > Change-Id: Ie005fa72314b8778c889969854bfb161e39d3178
    > > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/413004
    > > Commit-Queue: Matthew Boetger <boetger@google.com>
    > > Reviewed-by: Andrew Davies <awdavies@google.com>
    > > Testability-Review: Andrew Davies <awdavies@google.com>
    >
    > TBR=raggi@google.com,awdavies@google.com,boetger@google.com,tbodt@google.com,jwing@google.com
    >
    > Change-Id: I5e04cdb0e434b28e6653e22acdde5d80705821a8
    > No-Presubmit: true
    > No-Tree-Checks: true
    > No-Try: true
    > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414005
    > Reviewed-by: Matthew Boetger <boetger@google.com>
    > Commit-Queue: Matthew Boetger <boetger@google.com>
    
    TBR=raggi@google.com,awdavies@google.com,boetger@google.com,tbodt@google.com,jwing@google.com
    
    Change-Id: Id8fc0aa48e11b00cb319334eb981ff46616d7655
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414128
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Matthew Boetger <boetger@google.com>

commit 8abfa37ba637619129f2554d3513dd1b7baad0f9
Author: Matthew Boetger <boetger@google.com>
Date:   Wed Aug 5 22:23:42 2020 +0000

    Revert "[ffx] remove ffx_plugin_suite - just use ffx_plugin"
    
    This reverts commit b51c52307878dbfec0baef653d9ef088dc5d6715.
    
    Reason for revert: python breaks users using python3
    
    Original change's description:
    > [ffx] remove ffx_plugin_suite - just use ffx_plugin
    >
    > This allows for subcommands that are an Option - so if no subcommand is
    > given, plugin code can execute on the top level.
    >
    > MULTIPLY: ffx_bin_test
    > MULTIPLY: ffx_lib_test
    > MULTIPLY: ffx_target_lib_test
    > MULTIPLY: ffx_daemon_plugin_lib_test
    > MULTIPLY: ffx_component_lib_test
    >
    > Change-Id: Ie005fa72314b8778c889969854bfb161e39d3178
    > Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/413004
    > Commit-Queue: Matthew Boetger <boetger@google.com>
    > Reviewed-by: Andrew Davies <awdavies@google.com>
    > Testability-Review: Andrew Davies <awdavies@google.com>
    
    TBR=raggi@google.com,awdavies@google.com,boetger@google.com,tbodt@google.com,jwing@google.com
    
    Change-Id: I5e04cdb0e434b28e6653e22acdde5d80705821a8
    No-Presubmit: true
    No-Tree-Checks: true
    No-Try: true
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/414005
    Reviewed-by: Matthew Boetger <boetger@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit b51c52307878dbfec0baef653d9ef088dc5d6715
Author: Matt Boetger <boetger@google.com>
Date:   Wed Aug 5 17:10:07 2020 +0000

    [ffx] remove ffx_plugin_suite - just use ffx_plugin
    
    This allows for subcommands that are an Option - so if no subcommand is
    given, plugin code can execute on the top level.
    
    MULTIPLY: ffx_bin_test
    MULTIPLY: ffx_lib_test
    MULTIPLY: ffx_target_lib_test
    MULTIPLY: ffx_daemon_plugin_lib_test
    MULTIPLY: ffx_component_lib_test
    
    Change-Id: Ie005fa72314b8778c889969854bfb161e39d3178
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/413004
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 4684cd6b48f8130ec41901f19c59551cf6ca2864
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 4 20:08:37 2020 +0000

    [ffx] support nested config remove
    
    Change-Id: I5dabf7dbf3a36dd9905a43a31ffe515c715d769c
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/411917
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 04133fae17154802cfcd33a6430c46ccc6f577ee
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 4 16:53:58 2020 +0000

    [ffx] support nested config set
    
    Change-Id: I433f42ef95cb7141d931ca3a70e2b2c6a25183fe
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/411893
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit b312bc5213d325da84c7138bc338c8fafa29b48e
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 4 04:42:56 2020 +0000

    [ffx] Support "get" with nested JSON config
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I43e0f35e5b74acac559cdf2bb35deb00aefadaaf
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/411209
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 3bc8b025c23b233c3de74932ea7674c6015edc5c
Author: Matt Boetger <boetger@google.com>
Date:   Tue Aug 4 02:09:47 2020 +0000

    [ffx] Get rid of unnecessary config.rs
    
    Move runtime configuration into the priority_config
    
    MULTIPLY: ffx_config_lib_test
    Change-Id: I0df1affa36713cabe91e1b07614bff9bd500c73e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/411115
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 7bf63d57628220608bb7f8549169facdcb59a3d3
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jul 31 22:09:24 2020 +0000

    [ffx] Get rid of heuristics
    
    Add a utility method to check for file existence.
    
    MULTIPLY: ffx_config_lib_test, ffx_daemon_lib_test
    Change-Id: I43a7c86f94979f873837dceac99541dd81654873
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/410962
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit ba47be1a0169db1eefe4ac176e14600b34f3e484
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jul 30 18:29:03 2020 +0000

    [ffx] Provide a way to pass in a strategy to apply to config values.
    
    Use this to map environment variables and search through lists.
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I783abaf96fc2aa106488b2f9acee187eef1d099b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/410436
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit 0fb576da5b49e6ad69a6f3dd89995a028a875e03
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jul 24 21:09:09 2020 +0000

    [ffx] config code health - use anyhow::Result and bail
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: Iaecdeec2cbfb043d05fcdfeac670b795363fff2f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/409268
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 43b3b6d584538c2b011a688cc04682d1aedebb58
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jul 24 19:22:14 2020 +0000

    [ffx] UX refactoring for ffx config
    
    New ffx config get looks like this:
    
    > fx ffx config get
    FFX configuration can come from several places and has an inherit
    priority assigned
    to the different ways the configuration is gathered. A configuration key
    can be set
    in multiple locations but the first value found is returned. The
    following output
    shows the locations checked in descending priority order.
    
    **********************************************************************
    Configuration set via the 'ffx --config' parameter.
    
    none
    
    **********************************************************************
    Configuration set via environment variables.
    
    "log-dir" checks the environment variable(s): FFX_LOG_DIR, HOME,
    HOMEPATH
    Value found: "log-dir" = "/home/boetger"
    
    "ssh-port" checks the environment variable(s): FUCHSIA_SSH_PORT
    No values found.
    
    "log-enabled" checks the environment variable(s): FFX_LOG_ENABLED
    No values found.
    
    **********************************************************************
    Persistent configuration saved in files in the current environment.
    
    User Configuration
    {
      "ssh-test": "whatever",
      "test": "booyah",
      "test2": "1"
    }
    
    Build Configuration: none
    
    Global Configuration
    {
      "ssh-test": "global"
    }
    
    Default Configuration
    {
      "log-enabled": false
    }
    
    **********************************************************************
    Configuration calculated from the environment when ffx is run.
    
    "ssh-priv" = "/home/boetger/src/fuchsia/.ssh/pkey"
    "ssh-pub" = "/home/boetger/src/fuchsia/.ssh/authorized_keys"
    
    **********************************************************************
    
    MULTIPLY: ffx_config_lib_test
    
    Change-Id: I8e31eaa211291c2b24b451b18eddf6d63301eb08
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/405816
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>

commit e3d4cf581768685ce16b411db6b7557e5b2cdaf0
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jul 24 01:54:37 2020 +0000

    [ffx] Use std::default::Default instead of DEFAULT_FFX
    
    Change-Id: Iec517c5da08f58ab5db0f1a429dc47879b2b85bc
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/410101
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit e3f69384ebe608310b7043ca34ead1ec90086bf8
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 22 21:14:57 2020 +0000

    [ffx] Add environment_file flag to set environment location from command
    line
    
    Change-Id: I27079d1c374efd3a67a7758999393e485730a731
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/409199
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 82537ecd71a6024723d7e0089f3a8a6c263d6710
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 22 05:56:25 2020 +0000

    [ffx] Add ASCENDD_SOCKET to config
    
    Change-Id: I74c191d54ebbf1b0a11d4afe03e2b634f4af9333
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/409255
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit d709af905c93725ba9872606ed10dc240646f877
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jul 16 18:27:31 2020 +0000

    [ffx] Update docs s/development-bridge/ffx
    
    Change-Id: I1504e679069b5f2fd021d9803add715f59d55a1e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/407694
    Reviewed-by: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit e63842a9f245f622ba6c8f1ddd61dd052d125417
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jul 16 01:03:41 2020 +0000

    [ffx] Move 'test' subcommand under 'component'
    
    Change-Id: I9b00c332af3fc27bdd4d2d83c6d902b346a212d1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/406697
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit f960c499a6581229e6576c3b5299245f7bbd68b3
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jul 16 00:55:41 2020 +0000

    [ffx] Move constants out of Core
    
    Change-Id: I9fa3dfc606d54ce3ce593744d13e537d902909cc
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/405384
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 2e12f5379ac738f95139cec7a5e26a77ae01ee91
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 15 20:41:17 2020 +0000

    [ffx] Create target suite
    
    MULTIPLY: ffx_reboot_lib_test, ffx_off_lib_test, ffx_list_lib_test
    
    Change-Id: Ia49f342c167ec1d3aa9a068c466f67085ddc2435
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/403776
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 5baf7d758e17ab8efa870796d3feb1b3e4cf7b4c
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 15 18:45:39 2020 +0000

    [ffx] Move ConfigLevel to Config Plugin - no need to be in core.
    
    Change-Id: I90c2a84934992dd13d26e9f72631278b8d415eb0
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/405434
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 2a020fa33fb4f1691fa53f5d4b2988239c062c36
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jul 9 22:56:25 2020 +0000

    [ffx] Move plugin code to run_test_suite instead of duplicating code
    
    Change-Id: Ic90d7bfb843ccf644e2af4c94e6cc4fe34b2aec1
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/402972
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Konstantin Pozin <kpozin@google.com>
    Reviewed-by: Ankur Mittal <anmittal@google.com>
    Testability-Review: Ankur Mittal <anmittal@google.com>

commit e71ec642c18680e0fa0d48eecdbeb571242bab19
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jul 1 00:10:40 2020 +0000

    [ffx] Create daemon plugin suite
    
    MULTIPLY: ffx_daemon_stop_lib_test, ffx_echo_lib_test
    
    Change-Id: I89ac9f9a426934c0b08ee61e73d4701267e2464b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/403499
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 97f9604cb7183c056bea175bc523dc8cbbc34daa
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 26 22:02:25 2020 +0000

    [ffx] Remove Test Manager from RCS
    
    Change-Id: Ief6e5274d75995dca67f7d3187e3cefba409161b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/400585
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    API-Review: James Tucker <raggi@google.com>

commit 15996033ed03a865c74ac4cc4bfc82af5a129438
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jun 16 21:37:48 2020 +0000

    [ffx] Add a target CLI param to allow target selection.
    
    Change-Id: If38b0935186a631c9ab8274ea60dc9905a47c370
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/397236
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Jordon Wing <jwing@google.com>
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 7b9a191cab6ec9f95afefa1c5c3e63b1491d27ab
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 12 23:25:54 2020 +0000

    [ffx] use an mapping to automatically get arbitrary proxies
    
    We can automatically generate proxies if the developers give use the
    selection strings via a mapping in the ffx_plugin attribute.
    
    MULTIPLY: ffx_core_impl_lib_test
    
    Change-Id: I8bf5df7161fe5c11422d7b5d8268779728fbee8c
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393835
    Testability-Review: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 477abd5b1fd67fccdaeb1a616c8df4f0826848d8
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jun 10 00:04:22 2020 +0000

    [ffx] Create composable ffx plugin suite
    
    This allows you to create nested commands via generated argh
    subcommands. This cl adds subcommands to the echo command, e.g. 'ffx
    echo daemon' and 'ffx echo cli'.
    
    Change-Id: I7f4876f3ef18fbf5b8183d26fca87214f959cad4
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393269
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 097d4a185382bed2bc9841f05cbe75dc951c9e90
Author: Matt Boetger <boetger@google.com>
Date:   Fri Jun 5 01:52:22 2020 +0000

    [ffx] Make config plugin
    
    Change-Id: I132bfb9473537c150e35cc945d4692f4556e1af6
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393316
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 76808fa246756936b295bf1a3311cc96efdc6543
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 4 22:47:27 2020 +0000

    [ffx] Remove unnecessary CLI struct
    
    Change-Id: If660a60c9942aa38cce652b9a088dce41d3155cd
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393313
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 226db2dbc5b4d4020b9dd6704043796d276dfec5
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 4 18:29:47 2020 +0000

    [ffx] Detect DaemonProxy param in ffx_plugin
    
    With the double-dispatch it's now possible to identify that a ffx_plugin
    takes a DaemonProxy instead of a RemoteControlProxy.
    
    Extending this method in future CLs should allow for ffx_plugins that
    take a number of arbitrary Proxies, and then use the new RCS selector
    interface to gather the proxies - generating all the boilerplate code.
    
    Change-Id: If52821aed9697706b151a70c86cdc8facdbe6b58
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393195
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 5c2feaf302dcbad339c13cf18b3da58e8c6ff003
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 4 17:29:03 2020 +0000

    [ffx] Begin internal documentation.
    
    This is a good start.  There still needs to be some documentation around
    the persistent configuration files, how to setup an environment, etc.
    Also, how to use the config macros in the library.  But since this was
    timeboxed, this is what I have so far.
    
    Change-Id: I920f31571ae272a8e5087f555929f7152103e439
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/394187
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit b5044e41f7e1761d595393caadaad3cd97db2be8
Author: Matt Boetger <boetger@google.com>
Date:   Thu Jun 4 17:17:11 2020 +0000

    [ffx] Fix plugin tests names.
    
    This would provide collisions if there are multiple plugins in the same
    folder.
    
    Change-Id: Iabef2645a18667b8856c29fac385b9bcf774e1ba
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/395294
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit b4085a0f2702271c924169b7f55df798ec8d0738
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jun 3 17:45:24 2020 +0000

    [ffx] Use double-dispatch to allow for greater control in the plugins
    
    By passing the CLI into the plugin and allowing the macro to figure out
    how to get the remote control proxy, this opens up the plugins to be
    able to accept a DaemonProxy as the first parameter instead of the
    RemoteControlProxy.
    
    Change-Id: I06d6ceab9c4d94c049da9c6d451dc82e7268f20b
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/393154
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 58463d393491cbd49ef4d343dd58361fc8a1b761
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 28 23:18:17 2020 +0000

    [ffx] Fastboot discovery
    
    Change-Id: I8a05bab8e0920e39c61586b9837b135cf3d47bd2
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/392699
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit d79ed6783e71711725dcd7cdf58a9fbece55b21e
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 27 17:43:30 2020 +0000

    [ffx] Connect usb_bulk lib to fastboot lib
    
    Initial ffx fastboot lib code.
    
    Change-Id: I412bb7550500f8b50af11982a567327d7051b29f
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/388866
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit e8745538b2c8b7e1892f2ccd090563bbad1ecaa8
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 20 23:10:39 2020 +0000

    [ffx] Move argh stuctures to core
    
    This simplifies the build.
    
    Change-Id: Idd2afb18c097378c3999e2cdb2a76e64f39e7c72
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/391618
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 2a028371118933ecbdde3fbeaf437ca85c381396
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 20 22:27:59 2020 +0000

    [ffx] Move daemon code into it's own library
    
    Combines the ffxlib and daemon code all into one.
    
    MULTIPLY: ffx_bin_test, ffx_daemon_lib_test
    
    Change-Id: Iea6c27413fc98d6a8802e4751c69fef18f9db3a7
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/391636
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>

commit 0d62f0dd46b3468d39a81b8ab9331705afd729c1
Author: Matt Boetger <boetger@google.com>
Date:   Tue May 19 18:48:55 2020 +0000

    [ffx] Allow plugin args file to be passed in via param
    
    The ffx_plugin template now takes a param to identify the source for
    argh command structure.  This should allow multiple plugins per
    directory.
    
    MULTIPLY: ffx_test_lib_test, ffx_test_args_lib_test, ffx_bin_test
    
    Change-Id: I958c8706310aa2d54c80d6fbb02689a8035e86ce
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/391133
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 5a68823b35634b3516fc87698759cec6f45f811b
Author: Matt Boetger <boetger@google.com>
Date:   Mon May 18 21:23:33 2020 +0000

    [ffx] Ensure persistent config files are not used during unit tests
    
    Fix for fxb/52095
    
    MULTIPLY: ffx_config_lib_test, ffx_bin_test
    
    Change-Id: Id8b006b7a37c13a2d8b4936771bfbab5a32012e8
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/389823
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 9abc3e9093b3af21f0b7190668b7246a3b244281
Author: Matt Boetger <boetger@google.com>
Date:   Fri May 15 01:22:33 2020 +0000

    [ffx] Regen code if the template changes.
    
    Otherwise, this requires a clean and rebuild to get changes from the
    template into the build.
    
    Change-Id: Iaafa61fa705d967b6b57e56d51c1e0433a6eb3f5
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/390399
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit c322301f03618853aee3f0954da3d4abf2abba86
Author: Matt Boetger <boetger@google.com>
Date:   Thu May 14 23:21:44 2020 +0000

    [ffx] Remove unused subcommand and ffx command.
    
    These changes made it back in during a rebase.  This should not be
    here.
    
    MULTIPLY: ffx_bin_test, ffx_args_lib_test
    
    Change-Id: I653e6fe2736f23888e54655b133bb4cffcf09be9
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/390367
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 039583dd8aaf66c302a6bc65907c914b40611170
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 13 05:49:50 2020 +0000

    [ffx] Use attribute for plugins
    
    Reduced CLI integration to the following steps:
        1.) create ffx_plugin project with a lib.rs and args.rs
        2.) add plugin project to dependencies of ffx
        3.) decorate command struct in args.rs with ffx_command attribute
        4.) decorate method in lib.rs with ffx_plugin attribute
    
    Change-Id: I76f49be8a7bfeae93ef3c806c94b5bb1a9154109
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/388814
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 8425d1cf153b84478e0f4c3ecd60b0857690eb3e
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 13 05:39:50 2020 +0000

    [ffx] Code generation for plugin calls
    
    Reduced CLI integration to the following steps:
    1.) create ffx_plugin project with a lib.rs and args.rs
    2.) add plugin project to dependencies of ffx
    3.) add command type to args.rs (to be replaced with attribute)
    4.) add ffx_plugin method to lib.rs (to be replaced with attribute)
    
    Change-Id: I2a411b59a18679a9144bcd068b266501ee11a972
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/387934
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 957fac99ad85735c23dc2b98fa0782ebb6da9bbc
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 13 04:49:36 2020 +0000

    [ffx] Code generation for CLI argh struct
    
    Reduced CLI integration to the following steps:
    1.) create ffx_plugin project with a lib.rs and args.rs
    2.) add plugin project to dependencies of ffx
    3.) Add command type to args.rs (to be replaced with attribute)
    4.) register the plugin in the plugins.rs file
    
    Change-Id: Ie84ce3b5a11c54f807b5ef980068c0fd4d0c6baf
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/386850
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit 13eaff5b00459d1578de91799f403798d8815a54
Author: Matt Boetger <boetger@google.com>
Date:   Tue May 12 21:47:41 2020 +0000

    [ffx] Use macro and build rules for CLI integration
    
    Reduced CLI integration to the following steps:
    1.) create ffx_plugin project with a lib.rs and args.rs
    2.) add plugin project to dependencies of ffx
    3.) add the command created in args.rs to the Subcommand struct
    4.) register the plugin in the plugins.rs file
    
    I tried real hard to combine 3 and 4 - and I think with a little more
    refactoring it can get there .
    
    Change-Id: Ic9d8ad2b85c4e7c9aafbdb7a854f66e82a9f6212
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/385194
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit fceab88b8b261e5a662a9b534d3a14243e0afaaf
Author: Matt Boetger <boetger@google.com>
Date:   Tue May 12 20:48:31 2020 +0000

    [ffx] Cli refactor - organize more libraries.
    
    Config now works in the library world - adding macros to more easily
    overload the API.
    
    Change-Id: I423f12aa671853568701a8d88328a0366d3b106e
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/385233
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit ef70fb807e9b002b2179ee2862b0c1f9056f1d8c
Author: Matt Boetger <boetger@google.com>
Date:   Wed May 6 08:18:37 2020 +0000

    [ffx] CLI refactor - move integrations to their own libraries.
    
    This is the first step to start to understand the API necessary for
    developers to integrate with the CLI.
    
    Change-Id: I2e0f880579a2b82d3b6772edff3822145af45986
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/384921
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit b12451be42ce51d97f2284799e39047cbfb8420a
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 30 21:11:46 2020 +0000

    [ffx] Add a default.json file for default config
    
    Change-Id: I197d906822a392b110c02b7679a5aea7a90f8aab
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/383205
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 787a2ad23766775d3b49b90cee3afa430d86504f
Author: Matt Boetger <boetger@google.com>
Date:   Thu Apr 30 19:52:23 2020 +0000

    [ffx] Fix for config cache panic.
    
    Change-Id: I73334d19ff3d3f51f615104c30544f57608901ae
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/384257
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit bfcc9ff753437bedf0b27160ac149a1b4375250a
Author: Matt Boetger <boetger@google.com>
Date:   Wed Apr 29 17:42:11 2020 +0000

    [ffx] Remove compose - Daemon returns remote_proxy to Cli.
    
    RCS now handles multiple concurrent connections at once now as well.
    
    Change-Id: Iede4fa205393333dadd5f965559a5285b4df0a9d
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/383521
    API-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Testability-Review: Andrew Davies <awdavies@google.com>

commit f86f28a5d08cd220f8a5c8026692466ff2d5f511
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 27 19:40:22 2020 +0000

    [ffx] Adding a thread-safe cache for the Config
    
    This will prevent the config reloading everytime there's a query for a
    config key.
    
    Change-Id: Ibfb0e97f50c12d19193a00ea495b41a7759b5f50
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/381737
    Reviewed-by: Jordon Wing <jwing@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 4033a137edc5bed010af7f42f656784c2ba4e098
Author: Matt Boetger <boetger@google.com>
Date:   Tue Apr 21 19:36:43 2020 +0000

    [ffx] Config refactoring for code health.
    
    The one large configuration file was split into multiple files.  The API
    now distinguishes between ReadConfig and WriteConfigs.
    
    Change-Id: I25916fda311148430b3c6535879c0d10104dd965
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/381346
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 8bce3e77dc4e5866852b3999637dfc3a23f78f66
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 20 22:16:01 2020 +0000

    [ffx] Allow configuration to be passed in via a CLI parameter.
    
    There's also some clean up in this one.
    
    Change-Id: Id5d82325d0a26eac7c953f60ff970f4027a05cef
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/379390
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit c8ba93ea0d5f7109ec64d5c41ed5f3ca20eb57b7
Author: Matt Boetger <boetger@google.com>
Date:   Mon Apr 20 19:56:16 2020 +0000

    [ffx] Add environment variables to the ffx configuration
    
    Change-Id: Ibcf99f82aa2273ae0b25688e978ec36aa5ac42a2
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/379204
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit fc6ab0df43d604b0fc7eea64769e0fd948b383a8
Author: Matt Boetger <boetger@google.com>
Date:   Fri Apr 17 22:52:14 2020 +0000

    [ffx] Simplelog implementation
    
    Change-Id: Ia5337b6906ad864c801b1be815da925edac75f30
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/378766
    Testability-Review: James Tucker <raggi@google.com>
    Reviewed-by: Craig Tiller <ctiller@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit b5e78720f634ef83459b9a32381ff47b158e6d6c
Author: Matt Boetger <boetger@google.com>
Date:   Wed Apr 15 17:20:19 2020 +0000

    [third_party] Adding simplelog to third_party
    
    Context: ffx needs an implementation for the log facade to write to log files on the host side.
    
    OSRB Approval: fxb/49672
    
    Change-Id: I27ab6433ccc581f2096514e29283b98402095c50
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/378765
    Reviewed-by: Tyler Mandry <tmandry@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 02f76a13eef3262ada6a280b078f95c97ed1813c
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 31 05:14:24 2020 +0000

    [ffx] Test the output for ffx test with selectors
    
    Change-Id: Iaf769c55733caebab0a4f5ca2232e7c79926da07
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/376641
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Reviewed-by: James Tucker <raggi@google.com>
    Testability-Review: James Tucker <raggi@google.com>

commit 5d3969bb9802579e45a324b216005f8a1b3cc570
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 31 01:23:01 2020 +0000

    [ffx] Use a writer to print to stdout so we test output in unit tests
    
    Change-Id: If05e4c306773c21e0e4961bc1dac18535b97a561
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/375447
    Commit-Queue: Matthew Boetger <boetger@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Reviewed-by: Jordon Wing <jwing@google.com>
    Reviewed-by: Andrew Davies <awdavies@google.com>

commit 98279c38255b36c55905a522f9fe4481ab58ee09
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 31 00:17:49 2020 +0000

    [ffx] FTF Wildcard selection for running tests.
    
    Change-Id: I6b7f0ea7946124c94baf487719f425824367f802
    Reviewed-on: https://fuchsia-review.googlesource.com/c/fuchsia/+/375233
    Reviewed-by: James Tucker <raggi@google.com>
    Reviewed-by: Ankur Mittal <anmittal@google.com>
    Testability-Review: James Tucker <raggi@google.com>
    Commit-Queue: Matthew Boetger <boetger@google.com>

commit 3655eef2d8e72e4f3ebe0e1f2bcd2d6c2e245fa1
Author: Matt Boetger <boetger@google.com>
Date:   Tue Mar 24 19:00:50 2020 +0000

    [ffx] FTF Run Tests
    
    This requires cross-compiling the test_executor for both host and target
    builds.
    
    Change-Id: Ice97c0a8c0c5f91e823188b112e7034f9680959e

commit ea916d259c0b41334d1208068e7947cf3c232c01
Author: Matt Boetger <boetger@google.com>
Date:   Thu Mar 19 00:50:34 2020 +0000

    [ffx] FTF integration using the test manager Harness protocol.
    
    Change-Id: Icf075f4295298c6cb41ca4f3788beeb3073fd118

commit 9deaa8a90b3de4feedb6f816cff317c73f832fac
Author: Matt Boetger <boetger@google.com>
Date:   Mon Mar 9 21:50:54 2020 +0000

    [ffx] Add Heuristics to config
    
    Change-Id: Ifde1f8ebacd84800c3bb44df375c44c61bf5a6c8

commit 229eb0ca619dfa499562a557f374344e3fdf1420
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 21 19:14:58 2020 +0000

    [ffx] Implement config remove
    
    Change-Id: I5324a130afaee201c4e0274d0abe2cf26b762c2a

commit 2584115e68b3912fbb88c54008fed35774ebfff3
Author: Matt Boetger <boetger@google.com>
Date:   Fri Feb 21 18:05:23 2020 +0000

    [ffx] Connect the Config implementation to the user
    
    Change-Id: I89f3364f28a1f9a8674eca2e77cd6d9d751ad985

commit 6ea97b2a434e7ac17269eef1f04f64d165ef0580
Author: Matt Boetger <boetger@google.com>
Date:   Thu Feb 20 03:17:42 2020 +0000

    [ffx] Fix fastboot unused import.
    
    Change-Id: Ia647c8f89473b631325a84ec0143892e1794619b

commit 24eff62c3e5f40798093bb9bbf965a8ec61ffea8
Author: Matt Boetger <boetger@google.com>
Date:   Wed Feb 19 18:46:43 2020 +0000

    [ffx] Fastboot protocol client implementation
    
    Implement a simply fastboot client with io::Read, io::Write for
    transport to be filled in later.
    
    Change-Id: I8396d530b9319ac6bb257480c3e96bad189eebbe

commit 8770827b0c0ffc344a7bdb1508f35c44a9ac3f5a
Author: Matt Boetger <boetger@google.com>
Date:   Wed Feb 12 21:04:03 2020 +0000

    [ffx] Auto start the fdb daemon.
    
    Change-Id: I62968e7ff85821eb155b2dda9a0f59d7cc4223ff

commit e0a78f72e286035f2485e5fefa89d213ed552be4
Author: Matt Boetger <boetger@google.com>
Date:   Tue Feb 11 01:52:57 2020 +0000

    [ffx] Add a persistence layer to the config implementation.
    
    Change-Id: Iae7af6ca50ba954556b00255cb39d56cb3d40aaf

commit 348af745e1c7a6301d3acc71c57b84711177e772
Author: Matt Boetger <boetger@google.com>
Date:   Mon Feb 10 20:32:44 2020 +0000

    [ffx] Config API
    
    Defining the API and the prioritization scheme for different configs.
    After this, the persistentence layer will be added that handles the IO
    
    Change-Id: Ia5d8690b3eebc3424ca7abad05184b51b22438e4

commit 624e4e8269ecc953b92c9686ad91df1ad0fac86e
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jan 29 01:59:38 2020 +0000

    [Ffx] Rename fdb to ffx
    
    Change-Id: I892614573d1dd2ea4166891d3021d92bd0ba8740

commit 71ad82fc549588b517fa6ad36b42c0e279131e6e
Author: Matt Boetger <boetger@google.com>
Date:   Tue Jan 28 23:50:01 2020 +0000

    [ffx] Fastboot protocol implementation
    
    This just contains the byte vector to enum parsing for Commands and
    Replies as defined here:
    https://android.googlesource.com/platform/system/core/+/master/fastboot/
    
    Change-Id: Ibe332686f28aced0d3b5e9947c734f234fd20ea5

commit b26ea1568a22f600009d0cbdc5e7ece3b3002fcf
Author: Matt Boetger <boetger@google.com>
Date:   Wed Jan 15 20:32:10 2020 +0000

    [fdb] Remove daemon binary and just use the same binary for everything.
    
    Change-Id: Ic0eb704030fe79c6802a6732b1f75c80fa0b2cf0

commit c57e145dbd7e433b9a2d268e782b6a23d8f426cd
Author: Matt Boetger <boetger@google.com>
Date:   Sat Jan 11 03:55:29 2020 +0000

    [fdb] Add the remote control service to cli daemon.
    
    Change-Id: I249b25415be068b57d6e53dbb3ef524febf9ce84

commit c95eb3f4704bd39795edc568c958d6cadf541281
Author: Matt Boetger <boetger@google.com>
Date:   Fri Dec 13 23:42:22 2019 +0000

    [fdb] Create daemon
    
    Change-Id: I4189ff326a0eb4984f732bc7c40430d287d4a21a

commit 7a1f53adfc3b6a8769ab6eebecc0d07c62300d61
Author: Matt Boetger <boetger@google.com>
Date:   Tue Nov 19 18:05:13 2019 +0000

    [fdb] Adding initial fdb
    
    Change-Id: I7c024326b6cf2b46a60e1a997f6fffd988ab955a
